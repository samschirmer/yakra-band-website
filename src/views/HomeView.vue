<template>
  <div class="home content">

    <div class="columns">

      <div id="cover" class="column is-half">
        <figure class="image">
          <img src="@/assets/images/infinityd_cover.webp"/>
        </figure>
      </div>

      <div class="column is-half code">
        <code>
          infinityd: lp = {
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;1: "<RouterLink class="track-link" to="track/black-ocean">Black Ocean</RouterLink>",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;2: "<RouterLink class="track-link" to="track/modulo">Modulo</RouterLink>",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;3: "<RouterLink class="track-link" to="track/warning-of-the-goats">Warning of the Goats</RouterLink>",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;4: "<RouterLink class="track-link" to="track/return-ok">return !ok</RouterLink>",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;5: "<RouterLink class="track-link" to="track/coalescence">Coalescence</RouterLink>",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;6: "<RouterLink class="track-link" to="track/fork">fork()</RouterLink>",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;7: "<RouterLink class="track-link" to="track/sigkill">SIGKILL</RouterLink>",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;8: "<RouterLink class="track-link" to="track/evergreen">Evergreen</RouterLink>",
            <br />
          }
        </code>
      </div>

    </div>

  </div>
</template>

<style scoped>
.code {
  min-width: 450px;
  display: flex;
  align-items: center;
}
code {
  font-family: monospace;
  font-size: 12pt;
  color: #33ff00;
  background-color: rgba(0, 0, 0, 0);
  margin-bottom: 24px;
}

.image {
  max-width: 650px;
  max-height: 650px;
}

@media (min-width: 1024px) {
  .home {
    min-height: 100vh;
    margin-top: 120px;
  }
}
</style>
