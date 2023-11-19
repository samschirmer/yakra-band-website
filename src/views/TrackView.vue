<template>
  <div class="music content">
    <div class="columns">

      <div id="cover" class="column is-half">
        <figure class="image">
            <img :src="trackImg" :alt="title">
        </figure>
      </div>

      <div id="cover" class="column is-half">
        <p>
          #############<br />
          # {{ title }}<br />
          #############
        </p>
        <p><span v-html="lyrics"></span></p>
      </div>

    </div>
  </div>
</template>

<script>
import { ref, watch, computed } from 'vue';
import { useRoute } from 'vue-router';
import tracksData from '@/assets/lib/tracks.json';

export default {
  setup() {
    const route = useRoute();
    const trackImg = ref(null);
    const title = ref(null);
    const lyrics = ref(null);

    const slug = computed(() => route.params.trackName);

    const tracks = ref(tracksData);
    const track = computed(() => tracks.value[route.params.trackName] || {'title': 'infinityd', 'lyrics': ''});

    watch(slug, async (newVal, oldVal) => {
      if (newVal !== oldVal) {
        try {
          const imageModule = await import(`@/assets/images/${newVal}.png`);
          trackImg.value = imageModule.default;

          title.value = track.value.title
          lyrics.value = atob(track.value.lyrics)

        } catch (e) {
          console.error(e);
          trackImg.value = null;
        }
      }
    }, { immediate: true });
    return { trackImg, title, lyrics };
  }
};
</script>

<style>
@media (min-width: 1024px) {
  .music {
    padding-top: 60px;
    margin-top: 60px;
    min-height: 100vh;
    padding-bottom: 100px;
  }
}
</style>
