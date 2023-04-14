<script>
  import CardsList from '../assets/data/dc-comics.json'
  export default {
    name: "CardContainer",
    data() {
      return {
        CardsList,
      }
    }
  }
</script>

<template>
  <CardElement></CardElement>
</template>