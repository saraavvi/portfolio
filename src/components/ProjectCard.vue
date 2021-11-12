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
  height: 400px;
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
    padding: 3rem;

    .heading {
      font-family: $font-secondary;
      font-size: 5rem;
      margin-bottom: 2rem;
    }
  }
}
</style>
