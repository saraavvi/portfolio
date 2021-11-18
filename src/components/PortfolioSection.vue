<template>
  <section id="portfolio">
    <ProjectCard
      class="project-card"
      v-for="project in projects"
      :key="project"
      :name="project.name"
      :image="project.image"
      :description="project.description"
      :githubLink="project.githubLink"
      :hostedLink="project.hostedLink"
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
            "I created this simple weather app to practice working with React, but also because I wanted to practice using external APIs. In this app I worked with openWeatherMap API to display the weather forecast for the next 5 days. The user can search for a city and get a forecast! ",
          image: "weather-forecast",
          name: "Weather Forecast",
          githubLink: "https://github.com/saraavvi/weather-forecast-app",
          hostedLink: "https://saraavvi.github.io/weather-forecast-app/",
        },
        manCave: {
          description:
            "The mancave shop was a school assignment where the task was to create a webshop in plain PHP, using OOP and implementing the MVC concept. We used MySQL for storing all the data. A user can login, add producs to a shopping cart and place an order. There is also an admin interface for handling products and orders.   ",
          image: "mancave",
          name: "Mancave",
          githubLink: "https://github.com/saraavvi/mancave",
          hostedLink: "https://mancave-shop.herokuapp.com/",
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
