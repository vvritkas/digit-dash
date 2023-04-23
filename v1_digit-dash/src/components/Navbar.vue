<template>
  <nav class="navbar" role="navigation" aria-label="main navigation">
    <div class="navbar-brand">
      <a href="#">
        <img class="navbar-logo" src="/Digit-Dash-Logo.png" />
      </a>

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
        <a class="navbar-item button is-light"> How to play </a>

        <a class="navbar-item button is-info"> Highscore List </a>
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
  margin: 10px auto;
  position: sticky;
  top: 0;
}

.navbar-logo {
  height: 50px;
  width: auto;
}
.navbar-item {
  margin: 5px;
}
</style>
