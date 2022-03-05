<template>
  <footer>
      <FooterTop/>
      <FooterBottom/>
  </footer>
</template>

<script>
import FooterTop from './partials/FooterTop.vue';
import FooterBottom from './partials/FooterBottom.vue';
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