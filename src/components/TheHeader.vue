<template>
  <nav class="nav">
    <div class="links-container">
      <a class="logo" href="#landing"
        ><img class="logo" src="/images/logo2.png"
      /></a>
      <a class="nav-link" href="#about">About</a>
      <a class="nav-link" href="#portfolio">Portfolio</a>
      <a class="nav-link" href="#contact">Contact</a>
    </div>
  </nav>
</template>

<style scoped lang="scss">
.nav {
  padding: 2rem;
  margin: 0 auto;
  position: sticky;
  top: 0;
  background-color: $color-background;
  z-index: 1000;

  @include respond(phone) {
    padding: 0;
  }

  .links-container {
    width: 100%;
    align-items: center;
    display: flex;
    justify-content: center;

    .logo {
      height: 5rem;
      margin-right: auto;

      @include respond(phone) {
        display: none;
      }
    }
    .nav-link {
      @include hover-underline($color-secondary);
      font-size: 1.9rem;
      padding: 1rem 5rem;
      font-weight: bold;

      @include respond(phone) {
        padding: 2rem;
      }
    }
  }
}
</style>
