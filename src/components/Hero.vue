<script lang="ts" setup>

</script>

<template>
  <section class="hero">
    <div class="hero__container">
      <h1 class="hero-heading">Hi I'm <span class="hero-heading--highlight">Ismail Nyzar</span></h1>
      <p>I'm a webDeveloper</p>
      <p class="hero__description">Description Coming Soon :)</p>
      <p>Check out my code till that :P</p>
      <router-link class="hero__btn" to="/about">Learn More</router-link>
      <router-link class="hero__btn" to="/todo">Todo App</router-link>
      <router-link class="hero__btn" to="/socials">Socials</router-link>

    </div>
  </section>
</template>

<style scoped>
.hero {
  background: var(--clr-primary-10);
  min-height: 100vh;
  display: grid;
  place-items: center;
}

.hero__container {
  text-align: center;
}

.hero-heading {
  font-size: 3rem;
  margin-bottom: 1rem;
}

.hero-heading--highlight {
  color: var(--clr-primary-5);
}

.hero__description {
  margin-bottom: 2rem;
}

.hero__btn {
  display: inline-block;
  background: var(--clr-primary-5);
  color: var(--clr-primary-10);
  padding: 0.75rem 1rem;
  border-radius: var(--radius);
  text-transform: uppercase;
  letter-spacing: var(--spacing);
  font-weight: 400;
  transition: var(--transition);
  cursor: pointer;
}

.hero__btn:hover {
  //background: var(--clr-primary-7);
  //color: var(--clr-primary-1);
}

@media screen and (min-width: 992px) {
  .hero-heading {
    font-size: 5rem;
  }
}

</style>