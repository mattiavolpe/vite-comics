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
      <div class="container">
        <CardContainer class="card_container"></CardContainer>
      </div>
    </section>
    <ExternalSites></ExternalSites>
  </main>

  <SiteFooter></SiteFooter>

</template>

<style lang="scss">
  #jumbotron_container {
    height: 300px;
    overflow: hidden;
  }

  .card_container {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    flex-wrap: wrap;
  }
</style>