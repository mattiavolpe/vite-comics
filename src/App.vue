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
  .card_container {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
    flex-wrap: wrap;
  }
</style>