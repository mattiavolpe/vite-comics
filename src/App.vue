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
      ],
      externalSites: [
        {
          img: "./src/assets/img/buy-comics-digital-comics.png",
          title: "Digital comics",
          link: "#",
        },
        {
          img: "./src/assets/img/buy-comics-merchandise.png",
          title: "DC merchandise",
          link: "#",
        },
        {
          img: "./src/assets/img/buy-comics-subscriptions.png",
          title: "Subscription",
          link: "#",
        },
        {
          img: "./src/assets/img/buy-comics-shop-locator.png",
          title: "Comic shop locator",
          link: "#",
        },
        {
          img: "./src/assets/img/buy-dc-power-visa.png",
          title: "DC power visa",
          link: "#",
        },
      ]
    }
  }
}
</script>

<template>

  <header class="d-flex align-items-center justify-content-center">
    <div class="container d-flex justify-content-between align-items-center h-100">
      <div class="left">
        <img src="./assets/img/dc-logo.png" alt="DC Logo">
      </div>
      <ul class="right d-flex h-100">
        <li v-for="(item, index) in menuItems" :class="index === 0 ? 'active' : ''" class="d-flex align-items-center mx-3 h-100">
          <a :href="item.url">{{ item.title.toUpperCase() }}</a>
        </li>
      </ul>
    </div>
  </header>

  <main>
    <section id="main_section" class="bg-dark">
      <div class="container">
        <h1 class="m-0 py-5 text-light">--&gt; Content goes here &lt;--</h1>
      </div>
    </section>
    <section id="external_sites">
      <ul class="container d-flex justify-content-between align-items-center py-5 text-light">
        <li v-for="site in externalSites" class="mx-4">
          <img height="70" :src="site.img" :alt="site.title.toUpperCase() + ' Image'" class="me-2">
          <a :href="site.link" class="text-light">{{ site.title.toUpperCase() }}</a>
        </li>
      </ul>
    </section>
  </main>

</template>

<style>
</style>