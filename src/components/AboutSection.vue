<template>
  <section id="about">
    <h2 class="heading">About me</h2>
    <div class="me-container">
      <div class="me-intro">
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod, a?
          Ullam, temporibus voluptates. Est ut unde labore nihil eum temporibus
          maiores esse quod dignissimos! Nostrum amet perspiciatis sint quia
          nam?
        </p>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod, a?
          Ullam, temporibus voluptates. Est ut unde labore nihil eum temporibus
          maiores esse quod dignissimos! Nostrum amet perspiciatis sint quia
          nam?
        </p>
      </div>
      <div class="me-part">
        <h3 class="heading-sub">I would describe myself as...</h3>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod, a?
          Ullam, temporibus voluptates. Est ut unde labore nihil eum temporibus
          maiores esse quod dignissimos! Nostrum amet perspiciatis sint quia
          nam?
        </p>
      </div>
      <div class="me-part">
        <h3 class="heading-sub">I want to...</h3>
        <p>
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Quod, a?
          Ullam, temporibus voluptates. Est ut unde labore nihil eum temporibus
          maiores esse quod dignissimos! Nostrum amet perspiciatis sint quia
          nam?
        </p>
      </div>
    </div>
    <div class="skills-container">
      <h3 class="heading-sub">Languages &amp; techniques I've used</h3>
      <ul class="skills-list">
        <li class="skills-item" v-for="skill in skills" :key="skill">
          {{ skill }}
        </li>
      </ul>
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
  text-align: center;
  border-radius: 2rem;
  padding: 6rem 0;

  @include hover-lift;

  .heading {
    margin-bottom: 4rem;
    font-size: 4rem;
    font-family: $font-secondary;
  }
  .heading-sub {
    font-size: 2.5rem;
    margin-bottom: 3rem;
    color: $color-font-black;
  }
  .me-container {
    align-items: center;
    display: flex;
    justify-content: space-between;
    padding: 0 7rem;
    margin-bottom: 6rem;

    .me-intro {
      flex: 1.5;
      color: $color-font-grey;
    }
    .me-part {
      padding: 0 5rem;
      flex: 1;
      color: $color-font-grey;
    }
  }
  .skills-container {
    display: flex;
    flex-direction: column;
    align-items: center;

    .skills-list {
      display: flex;
      width: 50%;
      justify-content: center;
      flex-wrap: wrap;
      list-style: none;
    }
    .skills-item {
      padding: 2rem;
      background-color: $color-pop-sunny;
      border-radius: 2rem;
      margin: 1rem;
    }
  }
}
</style>
