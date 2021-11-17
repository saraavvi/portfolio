<template>
  <section id="about">
    <img class="image" src="/images/me.jpeg" />
    <div class="about-info">
      <h2 class="heading">A little bit about me</h2>
      <p>
        Hi, my name is Sara and I am fullstack developer with a focus on the
        frontend. I am at the end of a two year program at Nackademin in
        Stockholm and currently doing my internship at a company where I get to
        learn about Vue, CSS/Sass and frontend in general. When I'm not coding I
        like to spend time in the kitchen cooking or eating something delicious.
        I love exercising and really enjoy to go on hikes, do some yoga or a
        sweaty hiit session at the gym.
      </p>
      <div class="about-skills">
        <h2 class="heading">Languages &amp; techniques I've used</h2>
        <ul class="skills-list">
          <li class="skills-item" v-for="skill in skills" :key="skill">
            {{ skill }}
          </li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  data() {
    return {
      skills: [
        "HTML",
        "CSS/Sass",
        "Javascript",
        "PHP",
        "React.js",
        "Bootstrap",
        "Vue.js",
        "Node.js",
        "Git",
        "Github",
        "Netlify",
        "Heroku",
        "MongoDB",
        "MySQL",
        "Wordpress",
      ],
    };
  },
};
</script>

<style scoped lang="scss">
#about {
  padding: 6rem 0;
  color: $color-font-grey;
  align-items: center;
  display: flex;
  justify-content: center;
  padding: 0 30rem;

  .image {
    height: 50rem;
    border-radius: 2rem;
    box-shadow: $box-shadow;
  }

  .about-info {
    padding-left: 10rem;
    min-width: 60rem;
    display: flex;
    flex-direction: column;
    justify-content: center;

    .about-skills {
      display: flex;
      flex-direction: column;
    }

    .heading {
      font-size: 2rem;
      padding: 2rem 0 1rem 0;
      color: $color-font-black;
      font-family: $font-secondary;
    }

    .skills-list {
      display: flex;
      flex-wrap: wrap;
      list-style: none;
    }

    .skills-item {
      padding: 0rem 3rem 1rem 0;
    }
  }
}
</style>
