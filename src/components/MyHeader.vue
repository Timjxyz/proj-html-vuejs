<template>
  <header>
      <HeaderTop/>
      <HeaderBottom/>

  </header>
</template>

<script>
import HeaderTop from './partials/HeaderTop.vue';
import HeaderBottom from './partials/HeaderBottom.vue';
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