<script>
import ExternalSites from './components/ExternalSites.vue';
export default {
  data() {
    return {
      activeItem: 0,
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
    }
  },
  components: {
    ExternalSites,
  }
}
</script>

<template>

  <header class="d-flex align-items-center justify-content-center bg-light">
    <div class="container d-flex justify-content-between align-items-center h-100">
      <div class="left">
        <img src="./assets/img/dc-logo.png" alt="DC Logo">
      </div>
      <ul class="right d-flex h-100">
        <li v-for="(item, index) in menuItems" :class="activeItem === index ? 'active' : ''" class="d-flex align-items-center mx-3 h-100" @click="activeItem = index">
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
    <ExternalSites></ExternalSites>
  </main>

  <footer>
    <section id="footer_links">
      <div class="container d-flex justify-content-between align-items-center">
        <div id="links" class="d-flex text-light">
          <div>
            <h4>DC COMICS</h4>
            <ul>
              <li><a href="#">Characters</a></li>
              <li><a href="#">Comics</a></li>
              <li><a href="#">Movies</a></li>
              <li><a href="#">TV</a></li>
              <li><a href="#">Games</a></li>
              <li><a href="#">Videos</a></li>
              <li><a href="#">News</a></li>
            </ul>
            <h4>SHOP</h4>
            <ul>
              <li><a href="#">Shop DC</a></li>
              <li><a href="#">Shop DC Collectibles</a></li>
            </ul>
          </div>
          <div class="mx-5">
            <h4>DC</h4>
            <ul>
              <li><a href="#">Terms Of Use</a></li>
              <li><a href="#">Privacy policy (New)</a></li>
              <li><a href="#">Ad Choices</a></li>
              <li><a href="#">Advertising</a></li>
              <li><a href="#">Jobs</a></li>
              <li><a href="#">Subscriptions</a></li>
              <li><a href="#">Talent Workshops</a></li>
              <li><a href="#">CPSC Certificates</a></li>
              <li><a href="#">Ratings</a></li>
              <li><a href="#">Shop Help</a></li>
              <li><a href="#">Contact Us</a></li>
            </ul>
          </div>
          <div>
            <h4>SITES</h4>
            <ul>
              <li><a href="#">DC</a></li>
              <li><a href="#">MAD Magazine</a></li>
              <li><a href="#">DC Kids</a></li>
              <li><a href="#">DC Universe</a></li>
              <li><a href="#">DC Power Visa</a></li>
            </ul>
          </div>
        </div>
        <div class="img_wrapper">
          <img height="400" src="./assets/img/dc-logo-bg.png" alt="DC Logo BG">
        </div>
      </div>
    </section>
    <div id="bottom_banner">
      <div class="container d-flex justify-content-between align-items-center">
        <button>SIGN-UP NOW!</button>
        <div class="d-flex align-items-center">
          <h4 class="m-0 me-5">FOLLOW US</h4>
          <ul class="d-flex align-items-center">
            <li>
              <a href="#">
                <img src="./assets/img/footer-facebook.png" alt="">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="./assets/img/footer-twitter.png" alt="">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="./assets/img/footer-youtube.png" alt="">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="./assets/img/footer-pinterest.png" alt="">
              </a>
            </li>
            <li>
              <a href="#">
                <img src="./assets/img/footer-periscope.png" alt="">
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>

</template>

<style>
</style>