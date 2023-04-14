<script>
  import CardsList from '../assets/data/dc-comics.json';
  import CardElement from './CardElement.vue';
  export default {
    name: "CardContainer",
    data() {
      return {
        CardsList,
      }
    },
    components: {
      CardElement,
    }
  }
</script>

<template>
  <div>
    <CardElement class="card_element" v-for="item in CardsList" :img="item.thumb" :title="item.series"></CardElement>
  </div>
</template>

<style lang="scss" scoped>
  .card_element {
    width: calc(100% / 6);
  }
</style>