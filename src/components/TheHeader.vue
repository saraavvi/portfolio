<template>
  <nav class="nav">
    <a class="logo" href="#landing">S</a>
    <div class="links-container">
      <a class="nav-link" href="#about">About</a>
      <a class="nav-link" href="#portfolio">Portfolio</a>
      <a class="nav-link" href="#contact">Contact</a>
    </div>
  </nav>
</template>

<style scoped lang="scss">
.nav {
  display: flex;
  padding: 0rem 16rem;
  position: sticky;
  top: 0;
  background-color: $color-background;
  z-index: 1000;

  @include respond(tab-port) {
    padding: 0 8rem 0 8rem;
  }
  @include respond(phone) {
    padding: 0;
  }

  .logo {
    font-size: 5rem;
    font-family: $font-secondary;

    @include respond(phone) {
      display: none;
    }
  }
  .links-container {
    align-items: center;
    flex: 1;
    display: flex;
    justify-content: center;
  }
  .nav-link {
    @include hover-underline($color-secondary);
    font-size: 1.7rem;
    padding: 1rem 5rem;
    font-weight: bold;

    @include respond(phone) {
      padding: 2rem;
    }
  }
}
</style>
