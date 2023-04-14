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
  <div class="card_element">
    <img :src="img" :alt="title + 'Image'">
    <h5>{{ title }}</h5>
  </div>
</template>