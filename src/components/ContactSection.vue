<template>
  <section id="contact">
    <div class="text-container">
      <h2 class="contact-text">Want to get in touch?</h2>
      <p class="contact-text">
        Connect with me on
        <span class="li-link"
          ><a href="https://www.linkedin.com/in/saraviktorsson/"
            >LinkedIn</a
          ></span
        >
        and send me a message.
      </p>
    </div>
  </section>
</template>

<style scoped lang="scss">
#contact {
  font-family: $font-secondary;
  display: flex;
  justify-content: center;
  padding: 14rem;

  .text-container {
    min-width: 60rem;
    max-width: 50%;
    text-align: center;
  }
  .contact-text {
    font-size: 5rem;
    font-weight: normal;
  }
  .li-link {
    position: relative;

    &:after {
      content: "";
      position: absolute;
      bottom: 1rem;
      display: block;
      background-color: $color-secondary;
      height: 0.7rem;
      width: 100%;
      left: 0;
      transition: 0.1s ease;
    }

    &:hover:after {
      transform: translateY(-2px);
    }
  }
}
</style>
