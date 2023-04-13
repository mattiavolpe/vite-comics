<script>
  import MenuItems from '../assets/data/MenuItems.js';
  export default {
    name: "SiteHeader",
    data() {
      return {
        activeItem: 0,
        MenuItems,
      }
    }
  }
</script>

<template>
  <header class="d-flex align-items-center justify-content-center bg-light">
    <div class="container d-flex justify-content-between align-items-center h-100">
      <div class="left">
        <img src="./../assets/img/dc-logo.png" alt="DC Logo">
      </div>
      <ul class="right d-flex h-100">
        <li v-for="(item, index) in MenuItems" :class="activeItem === index ? 'active' : ''" class="d-flex align-items-center mx-3 h-100" @click="activeItem = index">
          <a :href="item.url">{{ item.title.toUpperCase() }}</a>
        </li>
      </ul>
    </div>
  </header>
</template>