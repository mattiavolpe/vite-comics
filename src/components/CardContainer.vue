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
  <div class="card_container">
    <CardElement v-for="item in CardsList" :img="item.thumb" :title="item.series"></CardElement>
  </div>
</template>