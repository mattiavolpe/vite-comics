<script>
import SiteHeader from './components/SiteHeader.vue';
import CardContainer from './components/CardContainer.vue';
import ExternalSites from './components/ExternalSites.vue';
import SiteFooter from './components/SiteFooter.vue';

export default {
  data() {
    return {
    }
  },
  components: {
    SiteHeader,
    CardContainer,
    ExternalSites,
    SiteFooter,
  }
}
</script>

<template>

  <SiteHeader></SiteHeader>

  <main>
    <div id="jumbotron_container">
      <img class="img-fluid" src="./assets/img/jumbotron.jpg" alt="Jumbotron">
    </div>
    <section id="main_section" class="bg-dark">
      <div class="container text-center">
        <h4 class="current_series">CURRENT SERIES</h4>
        <CardContainer class="card_container"></CardContainer>
        <button class="load_more">LOAD MORE</button>
      </div>
    </section>
    <ExternalSites></ExternalSites>
  </main>

  <SiteFooter></SiteFooter>

</template>

<style lang="scss">
@use './assets/scss/partials/variables.scss' as *;
  #jumbotron_container {
    height: 300px;
    overflow: hidden;
  }

  .current_series {
    color: $light;
    background-color: $accent;
    width: max-content;
    padding: 0.5rem 1rem;
    transform: translate(0, -50%);
  }

  .card_container {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    flex-wrap: wrap;
  }

  .load_more {
    color: $light;
    background-color: $accent;
    font-weight: 500;
    border: none;
    padding: 0.5rem 5rem;
    margin-bottom: 2rem;
  }
</style>