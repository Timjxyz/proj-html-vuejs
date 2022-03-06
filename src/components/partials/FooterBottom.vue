<template>
  <div class="footer-bottom">
    <div class="container">
      <p>Enjoy the low price. We are tracking any intention of piracy.</p>

      <p><i class="fa-regular fa-copyright"></i>  2020 NEXGEN is Proudly Power by Codings.</p>
    </div>

    <i class="fa-solid fa-arrow-up"></i>

  </div>
</template>

<script>
export default {
    name:'FooterBottom'
}
</script>

<style lang="scss" scoped>
@import "../../assets/style-scss/variables.scss";

  .footer-bottom{
    background-color: #0d0d11;
    height: 80px;
    position: relative;

    .fa-arrow-up{
      position: absolute;
      right: 20px;
      top: 50%;
      transform: translateY(-50%);
      color:#0d0d11;
      background-color:#111619;
      line-height: 30px;
      text-align: center;
      height: 30px;
      width: 30px;
      border-radius: 50%;
      font-size: 20px;
      
    }

    .container{
      width: 70%;
      height: 100%;
      margin: 0px auto;
      display: flex;
      align-items: center;
      justify-content: space-between;
      color: $colorGravel;
      font-size: 14px;
      font-weight: 400;

      i{
        font-size: 10px;
      }
    }
  }

</style>