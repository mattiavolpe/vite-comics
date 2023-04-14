<script>
  export default {
    name: "CardElement",
    props: {
      img: String,
      title: String,
    }
  }
</script>

<template>
  <div>
    <img :src="img" :alt="title + 'Image'">
    <h5>{{ title }}</h5>
  </div>
</template>

<style lang="scss" scoped>
@use "../assets/scss/partials/variables" as *;
  img {
    width: 100%;
    aspect-ratio: 1 / 1;
    object-fit: contain;
    margin-top: 2rem;
  }

  h5 {
    color: $light;
    text-align: center;
    font-weight: 400;
    margin: 0.5rem 0 2rem; 
  }
</style>