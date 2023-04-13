<script>
import SiteHeader from './components/SiteHeader.vue';
import ExternalSites from './components/ExternalSites.vue';
import SiteFooter from './components/SiteFooter.vue';
export default {
  data() {
    return {
    }
  },
  components: {
    SiteHeader,
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
        <h1 class="m-0 py-5 text-light">--&gt; Content goes here &lt;--</h1>
      </div>
    </section>
    <ExternalSites></ExternalSites>
  </main>

  <SiteFooter></SiteFooter>

</template>