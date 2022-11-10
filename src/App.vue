<script>
import SiteHeader from './components/SiteHeader.vue';
import SiteMain from './components/SiteMain.vue';

export default {
  components: {
    SiteHeader,
    SiteMain
  }
}
</script>

<template>

  <SiteHeader />
  <!-- /#site-header -->
  <SiteMain />
  <!-- /#site_main -->
  <footer id="site_footer"></footer>
  <!-- /#site-footer -->

</template>

<style scoped>

</style>