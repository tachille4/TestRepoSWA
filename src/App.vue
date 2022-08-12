<script setup lang="ts">
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
import BannerItem from './components/BannerItem.vue'
</script>

<template>
  <header>
    <img alt="SWA logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld title="Static Web Apps" message="Welcome to my personal website!"/>
    </div>
  </header>

  <main>
    <TheWelcome />
  </main>

  <BannerItem>
    <template #heading>About Me</template>
    I'm a relatively young product helping developer build and deploy static website content. 
    Learn more about me through my <a target="_blank" href="https://docs.microsoft.com/en-us/azure/static-web-apps/">documention</a>.
  </BannerItem>

  <BannerItem>
    <template #heading>My Projects</template>
    Check out product updates and see what we offer to make your development experience.
  </BannerItem>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
