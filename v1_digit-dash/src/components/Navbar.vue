<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <RouterLink to="/">
        <img class="navbar-logo" src="/Digit-Dash-Logo.png" />
      </RouterLink>

      <a
        role="button"
        class="navbar-burger"
        aria-label="menu"
        aria-expanded="false"
        data-target="navbarBasicExample"
      >
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
        <span aria-hidden="true"></span>
      </a>
    </div>

    <div id="navbarBasicExample" class="navbar-menu">
      <div class="navbar-end">
        <RouterLink to="/howToPlay" class="navbar-item button is-light">
          How to play
        </RouterLink>

        <RouterLink to="/highscore" class="navbar-item button is-info">
          Highscore List
        </RouterLink>
      </div>
    </div>
  </nav>
</template>

<script>
export default {};
</script>

<style scoped>
.navbar {
  height: 50px;
  max-width: 1200px;
  margin: 5px auto;
  position: sticky;
  top: 0px;
}

.navbar-logo {
  height: 50px;
  width: auto;
}
.navbar-item {
  margin: 5px;
}
</style>
