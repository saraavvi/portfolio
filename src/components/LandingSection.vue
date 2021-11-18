<template>
  <section id="landing">
    <div class="heading-container">
      <h1 class="heading">
        Hello, I’m Sara.<br />
        A creative thinker and a problem solver.
      </h1>
      <p class="sub">
        I’m currently focusing on the frontend and design, but have experience
        in a broad set of areas such as backend and databas stuff.
      </p>
    </div>
  </section>
</template>

<style scoped lang="scss">
#landing {
  margin-top: 5rem;
  background-image: linear-gradient($color-primary, $color-secondary);
  border-radius: 2rem;
  display: flex;
  height: 75vh;
  justify-content: center;
  align-items: center;
  box-shadow: $box-shadow;

  @include respond(tab-port) {
    height: 85vh;
  }

  @include hover-lift;

  .heading-container {
    padding: 3rem;

    .heading {
      font-family: $font-secondary;
      font-size: 5rem;

      @include respond(phone) {
        font-size: 4rem;
      }
    }
    .sub {
      font-size: 2rem;
    }
  }
}
</style>
