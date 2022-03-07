<template>
  <footer>
      <FooterTop/>
      <FooterBottom/>
  </footer>
</template>

<script>
import FooterTop from './partials/partialsFooter/FooterTop.vue';
import FooterBottom from './partials/partialsFooter/FooterBottom.vue';
export default {
    name:'MyFooter',
    components:{
      FooterTop,
      FooterBottom
      
    }

}
</script>

<style>

</style>