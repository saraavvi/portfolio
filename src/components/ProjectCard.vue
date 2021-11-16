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
        <button class="button">Github</button>
        <button class="button">View it live</button>
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
  },
};
</script>

<style scoped lang="scss">
.project-container {
  border-radius: 2rem;
  height: 40rem;
  display: flex;

  @include hover-lift;

  .image-container {
    top: 3rem;
    height: 100%;
    padding: 3rem;

    .image {
      border-radius: 2rem;
      object-fit: contain;
      box-shadow: $box-shadow;
      height: 100%;
    }
  }
  .description-container {
    padding: 3rem 4rem;
    display: flex;
    flex-direction: column;

    .heading {
      font-family: $font-secondary;
      font-size: 5rem;
      margin-bottom: 2rem;
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
