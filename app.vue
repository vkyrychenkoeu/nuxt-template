<script setup lang="ts">
import './assets/base.css'
</script>
<template>
  <section>
    <header>
      <div class="hero-top">
        <img src='/fleekLogo.svg' height="87" />
        <img src='/plus.svg' />
        <img src='/logo.svg' height="87" />
      </div>

      <p class='description'>
        This is a template for creating a static site using Nuxt and deploying it on Fleek.
      </p>
    </header>

    <main>
      <ul role="list" class='card-list'>
        <Card href="https://docs.fleek.xyz/" title="Fleek Documentation"
          body="Learn about Fleek & the available services by cheking our official docs.">
          <img height="31" width="31" src="/fleekMark.svg" />
        </Card>

        <Card href="https://nuxt.com/" title="Nuxt Documentation"
          body="Learn about Nuxt in their official docs.">
          <img height="31" width="31" src="/logo.svg" />
        </Card>

        <Card href="https://blog.fleek.xyz/" title="Fleek Blog"
          body="Checkout our Blog for more information about Fleek.">
          <img height="31" width="31" src="/fleekMark.svg" />
        </Card>

        <Card href="https://nuxt.com/modules" title="Nuxt Modules"
          body="Explore modules to supercharge your Nuxt Project">
          <img height="31" width="31" src="/logo.svg" />
        </Card>
      </ul>
    </main>
  </section>
</template>

<style scoped>

section {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: auto;
  gap: 2rem;
  height: 100vh;
}

header {
  display: flex;
  align-items: center;
  flex-direction: column;
  gap: 2.5rem;
}

.hero-top {
  display: flex;
  align-items: center;
  gap: 50px;
  margin-left: -75px;
}

.description {
  font-size: 1.5rem;
  line-height: 2rem;
  text-align: center;
  width: 100%;
}

.card-list {
  display: grid;
  grid-template-columns: repeat(2, minmax(0, 1fr));
  gap: 15px;
}

main {
  width: 75%;
  display: flex;
  flex-direction: column;
  align-items: center;
  margin: 0 auto;
  gap: 2.5rem;
}
</style>
