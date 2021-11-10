<template>
  <section id="landing">
    <div class="heading-container">
      <h1 class="heading">
        Hello, I’m Sara.<br />
        A creative thinker and a problem solver.
      </h1>
      <p class="sub">
        I’m currently focusing on frontend and design but have experience in a
        broad set of areas such as backend and databas stuff.
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

  @include hover-lift;

  .heading-container {
    padding: 3rem;

    .heading {
      font-family: $font-secondary;
      font-size: 5rem;
    }
    .sub {
      font-size: 2rem;
    }
  }
}
</style>
