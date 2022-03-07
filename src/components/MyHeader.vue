<template>
  <header>
      <HeaderTop/>
      <HeaderBottom/>

  </header>
</template>

<script>
import HeaderTop from './partials/partialsHeader/HeaderTop.vue';
import HeaderBottom from './partials/partialsHeader/HeaderBottom.vue';
export default {
    name:'MyHeader',
    components:{
        HeaderTop,
        HeaderBottom
    }

}
</script>

<style>

</style>