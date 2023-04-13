<script>
export default {
  data() {
    return {
      menuItems: [
        {
          title: "Characters",
          url: "#",
        },
        {
          title: "Comics",
          url: "#",
        },
        {
          title: "Movies",
          url: "#",
        },
        {
          title: "TV",
          url: "#",
        },
        {
          title: "Games",
          url: "#",
        },
        {
          title: "Collectibles",
          url: "#",
        },
        {
          title: "Videos",
          url: "#",
        },
        {
          title: "Fans",
          url: "#",
        },
        {
          title: "News",
          url: "#",
        },
        {
          title: "Shop",
          url: "#",
        },
      ]
    }
  }
}
</script>

<template>

  <header class="py-4">
    <div class="container d-flex justify-content-between align-items-center">
      <div class="left">
        <img src="./assets/img/dc-logo.png" alt="DC Logo">
      </div>
      <ul class="right d-flex m-0">
        <li v-for="item in menuItems" class="mx-3">
          <a :href="item.url">{{ item.title.toUpperCase() }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>

<style>
</style>