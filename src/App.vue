<script setup>

import Banner from './components/Banner.vue'
import Section2 from './components/Section2.vue'
import Section3 from './components/Section3.vue'

</script>

<template>
  <header>

  </header>

  <main>
    <Banner/>
    <Section2/>
    <Section3/>


  </main>
</template>

<style scoped>
body{
  background-color: #fff !important;
}
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
