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
  padding: 0 16rem 0 16rem;
  position: sticky;
  top: 0;
  background-color: $color-background;
  z-index: 1000;

  .logo {
    font-size: 4rem;
    font-family: $font-secondary;
  }
  .links-container {
    align-items: center;
    flex: 1;
    display: flex;
    justify-content: center;
  }
  .nav-link {
    @include hover-underline;
    font-size: 1.7rem;
    padding: 1rem 5rem;
    font-weight: bold;
  }
}
</style>
