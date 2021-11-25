<template>
  <section id="about">
    <img class="image" src="/images/me.jpeg" />
    <div class="about-info">
      <h2 class="heading">✨ A little bit about me</h2>
      <p>
        Hi, my name is Sara and I am a fullstack developer student, eager to
        learn everything about frontend development. I am at the end of a two
        year program at Nackademin in Stockholm, and currently doing my
        internship at a company where, among other things, I get to learn about
        Vue &amp; CSS/Sass. When I'm not coding I like to spend time cooking or
        eating something delicious. I love exercising and really enjoy to go
        hiking, do some yoga, or workout at the gym.
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
  padding: 14rem 30rem;
  color: $color-font-grey;
  align-items: center;
  display: flex;
  justify-content: center;

  @include respond(desktop) {
    padding: 10rem 30rem;
  }
  @include respond(tab-port) {
    flex-direction: column-reverse;
    text-align: center;
    padding: 5rem 30rem 0 30rem;
  }
  @include respond(phone) {
    padding: 0;
  }

  .image {
    height: 50rem;
    border-radius: 2rem;
    box-shadow: $box-shadow;

    @include respond(tab-port) {
      height: 60rem;
      transform: rotate(-90deg);
    }
    @include respond(phone) {
      width: 70%;
      height: auto;
    }
  }
}

.about-info {
  padding-left: 10rem;
  min-width: 60rem;
  max-width: 60rem;
  display: flex;
  flex-direction: column;
  justify-content: center;

  @include respond(tab-port) {
    padding-left: 0;
    min-width: 60rem;
  }
  @include respond(phone) {
    min-width: 30rem;
  }

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

    @include respond(tab-port) {
      justify-content: center;
    }
  }

  .skills-item {
    padding: 0rem 3rem 1rem 0;
  }
}
</style>
