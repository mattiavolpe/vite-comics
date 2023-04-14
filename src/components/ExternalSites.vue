<script>
  import ExternalSites from '../assets/data/ExternalSites.js';
  export default {
    name: "ExternalSites",
    data() {
      return {
        ExternalSites,
      }
    },
    methods: {
      getImageUrl(img) {
        return new URL(`../assets/img/${img}`, import.meta.url).href;
      }
    }
  }
</script>

<template>
  <section id="external_sites">
    <ul class="container d-flex justify-content-between align-items-center py-5 text-light">
      <li v-for="site in ExternalSites" class="mx-4">
        <img height="70" :src="getImageUrl(site.img)" :alt="site.title.toUpperCase() + ' Image'" class="me-2">
        <a :href="site.link" class="text-light">{{ site.title.toUpperCase() }}</a>
      </li>
    </ul>
  </section>
</template>

<style>

</style>