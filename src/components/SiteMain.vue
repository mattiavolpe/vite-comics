<script>
  import CardContainer from './CardContainer.vue';
  import ExternalSites from './ExternalSites.vue';
  export default {
    name: "SiteMain",
    components: {
      CardContainer,
      ExternalSites,
    }
  }
</script>

<template>
  <main>
    <div id="jumbotron_container">
      <img class="img-fluid" src="../assets/img/jumbotron.jpg" alt="Jumbotron">
    </div>
    <section id="main_section" class="bg-dark">
      <div class="container text-center">
        <h4 class="current_series">CURRENT SERIES</h4>
        <CardContainer></CardContainer>
        <button class="load_more">LOAD MORE</button>
      </div>
    </section>
    <ExternalSites></ExternalSites>
  </main>
</template>