<template>
  <footer class="footer">
    <div class="has-text-centered">
      <p>
        &copy; {{ new Date().getFullYear() }} Yakra
      </p>
    </div>
    <div class="social has-text-right">
      <a href="https://instagram.com/Yakra" class="icon">
        <font-awesome-icon icon="fa-brands fa-instagram" size="2xl" style="color: #ffffff;"></font-awesome-icon>
      </a>
      <a href="https://youtube.com/Yakra" class="icon">
        <font-awesome-icon icon="fa-brands fa-youtube" size="2xl" style="color: #ffffff;"></font-awesome-icon>
      </a>
      <a href="https://spotify.com/Yakra" class="icon">
        <font-awesome-icon icon="fa-brands fa-spotify" size="2xl" style="color: #ffffff;"></font-awesome-icon>
      </a>
      <a href="https://spotify.com/Yakra" class="icon">
        <font-awesome-icon icon="fa-brands fa-soundcloud" size="2xl" style="color: #ffffff;"></font-awesome-icon>
      </a>
      <a href="https://yakra.bandcamp.com" class="icon">
        <font-awesome-icon icon="fa-brands fa-bandcamp" size="2xl" style="color: #ffffff;"></font-awesome-icon>
      </a>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'PageFooterComponent'
}
</script>

<style scoped>
.footer {
  align-items: center;
  justify-content: space-between;
  display: flex;
  padding: 12px;
  width: 100%;
  background-color: #0a0a0a;
  color: #4a4a4a;

  position: fixed;
  height: 70px;
  bottom: 0px;
  left: 0px;
  right: 0px;
  margin-bottom: 0px;
}

.social {
  margin-left: auto;
}

.icon {
  margin-left: 12px;
  margin-right: 12px;
}
</style>
