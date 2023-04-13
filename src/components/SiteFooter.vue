<script>
  import FooterLinks from './FooterLinks.vue';
  import BottomBanner from './BottomBanner.vue';
  export default {
    name: "SiteFooter",
    components: {
      FooterLinks,
      BottomBanner,
    }
  }
</script>

<template>
  <footer>
    <FooterLinks></FooterLinks>
    <BottomBanner></BottomBanner>
  </footer>
</template>