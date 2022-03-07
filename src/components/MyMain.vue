<template>
  <main>
      <FirstPMain/>
      <img class="top-img" src="../assets/svg/svg-0.svg" alt="">
      <SecondPMain/>
       <img class="bottom-img" src="../assets/svg/svg-0.svg" alt="">
        <ThirdPMain/>
        <FourthPMain/>
        <FifthPMain/>
  </main>
</template>

<script>
import FirstPMain from './partials/partialsMain/FirstPMain.vue';
import SecondPMain from './partials/partialsMain/SecondPMain.vue';
import ThirdPMain from './partials/partialsMain/ThirdPMain.vue';
import FourthPMain from './partials/partialsMain/FourthPMain.vue';
import FifthPMain from './partials/partialsMain/FifthPMain.vue';
export default {
    name:'MyMain',
    components:{
      FirstPMain,
      SecondPMain,
      ThirdPMain,
      FourthPMain,
      FifthPMain
      
    }
}
</script>

<style lang="scss" scoped>
  main{
    position: relative;
    img{
      position: absolute;
      left: 50%;
      transform: translate(-50%);
     
      filter: invert(72%) sepia(34%) saturate(590%) hue-rotate(131deg) brightness(86%) contrast(87%);
    }
    .top-img{   
      margin-top: -28px;
    }
    .bottom-img{
     margin-top: -28px;
    }

  }

</style>