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
            &nbsp;&nbsp;&nbsp;&nbsp;1: "Black Ocean",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;2: "Modulo",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;3: "Warning of the Goats",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;4: "return !ok",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;5: "Coalescence",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;6: "fork()",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;7: "SIGKILL",
            <br />
            &nbsp;&nbsp;&nbsp;&nbsp;8: "Evergreen"
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
