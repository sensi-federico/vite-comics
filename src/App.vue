<script>
import SiteHeader from './components/SiteHeader.vue';
import SiteMain from './components/SiteMain.vue';
import SiteFooter from './components/Sitefooter.vue';

export default {
  components: {
    SiteHeader,
    SiteMain,
    SiteFooter
  }
}
</script>

<template>

  <SiteHeader />
  <!-- /#site-header -->
  <SiteMain />
  <!-- /#site_main -->
  <SiteFooter />
  <!-- /#site-footer -->

</template>

<style scoped>

</style>