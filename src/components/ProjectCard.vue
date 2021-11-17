<template>
  <div class="project-container">
    <div class="image-container">
      <img class="image" :src="'/images/' + image + '.png'" />
    </div>
    <div class="description-container">
      <h2 class="heading">{{ name }}</h2>
      <p class="description">
        {{ description }}
      </p>
      <div class="button-container">
        <button class="button"><a :href="githubLink">Github</a></button>
        <button class="button">
          <a :href="hostedLink">View it live</a>
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    image: {
      type: String,
    },
    name: {
      type: String,
    },
    description: {
      type: String,
    },
    githubLink: {
      type: String,
    },
    hostedLink: {
      type: String,
    },
  },
};
</script>

<style scoped lang="scss">
.project-container {
  border-radius: 2rem;
  height: 40rem;
  display: flex;

  @include hover-lift;

  @include respond(tab-port) {
    flex-direction: column-reverse;
    height: auto;
  }

  .image-container {
    height: 100%;
    padding: 3rem;
    align-self: center;

    @include respond(desktop) {
      height: 95%;
    }
    @include respond(tab-land) {
      height: 70%;
    }
    @include respond(tab-port) {
      height: 50%;
      width: 100%;
    }

    .image {
      border-radius: 2rem;
      object-fit: contain;
      box-shadow: $box-shadow;
      height: 100%;

      @include respond(tab-port) {
        height: auto;
        width: 100%;
      }
    }
  }
  .description-container {
    padding: 3rem 5rem;
    display: flex;
    flex-direction: column;

    @include respond(desktop) {
      padding-left: 0rem;
    }
    @include respond(tab-land) {
      align-self: center;
    }
    @include respond(tab-port) {
      padding: 5rem;
    }

    .description {
      min-width: 40rem;
    }

    .heading {
      font-family: $font-secondary;
      font-size: 5rem;
      margin-bottom: 2rem;

      @include respond(desktop) {
        margin-bottom: 0rem;
      }
      @include respond(tab-land) {
        font-size: 4rem;
      }
    }
    .button-container {
      display: flex;
      justify-content: flex-end;
      margin-top: auto;
    }
    .button {
      @include hover-underline($color-pop-sunny);
      border: none;
      font-weight: bold;
      font-size: 1.7rem;
      padding: 1.5rem 2rem;
      cursor: pointer;
      font-family: inherit;
      background-color: inherit;
    }
  }
}
</style>
