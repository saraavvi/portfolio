<template>
  <section id="portfolio">
    <ProjectCard
      class="project-card"
      v-for="project in projects"
      :key="project"
      :name="project.name"
      :image="project.image"
      :description="project.description"
    />
  </section>
</template>

<script>
import ProjectCard from "./ProjectCard";
export default {
  data() {
    return {
      projects: {
        weatherForecast: {
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores a accusantium perspiciatis harum quisquam possimus tempora libero vel eius ullam, nostrum repellat eveniet optio corrupti labore. Vel soluta odio esse!",
          image: "weather-forecast",
          name: "Weather Forecast",
        },
        manCave: {
          description:
            "Lorem ipsum dolor sit amet consectetur adipisicing elit. Dolores a accusantium perspiciatis harum quisquam possimus tempora libero vel eius ullam, nostrum repellat eveniet optio corrupti labore. Vel soluta odio esse!",
          image: "mancave",
          name: "Mancave",
        },
      },
    };
  },
  components: {
    ProjectCard,
  },
};
</script>

<style lang="scss" scoped>
.project-card {
  margin-bottom: 10rem;
  box-shadow: $box-shadow;
}
</style>
