<template>
<!-- Prima sezione del main con elencati alcuni servizi  -->
  <section class="services">
    <div class="container">

      <!-- Titolo e testo dell asezione -->
      <div class="section-text">
        <h6>OUR BUSINESS AREAS</h6>
        <h2>Excellence in <span class="evidenziatore">Services</span></h2>
        <p>
          We are leaders in providing consultancy services with a 
          set of cutting-edge technologies and a team of experienced and renowned professionals. 
          These are some options that you can hire.
        </p>
        <div class=" btn btn-green">
          <a href="#"> SEE ALL</a>
        </div>

      </div>

      <!-- Contenuti box dei vari servizi -->

      <div class="box-container">
        <!-- Box 1 -->
        <div class="box">
          <img src="../../../assets/svg/svg-1.svg" alt="">
          <h3>Audit & Assurance</h3>
          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Error,  </p>
          <i class="fa-solid fa-arrow-right"></i>
        </div>

        <!-- Box 2 -->
        <div class="box">
          <img src="../../../assets/svg/svg-2.svg" alt="">
          <h3>Financial Advisory</h3>
          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Error,  </p>
          <i class="fa-solid fa-arrow-right"></i>
        </div>

        <!-- Box 3 -->
        <div class="box">
          <img src="../../../assets/svg/svg-3.svg" alt="">
          <h3>Analytics and M&A</h3>
          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Error,  </p>
          <i class="fa-solid fa-arrow-right"></i>
        </div>

        <!-- Box 4 -->
        <div class="box">
          <img src="../../../assets/svg/svg-4.svg" alt="">
          <h3>Middle Marketing</h3>
          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Error,  </p>
          <i class="fa-solid fa-arrow-right"></i>
        </div>

        <!-- Box 5 -->
        <div class="box">
          <img src="../../../assets/svg/svg-5.svg" alt="">
          <h3>Legal Consulting</h3>
          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Error,  </p>
          <i class="fa-solid fa-arrow-right"></i>
        </div>

        <!-- Box 6 -->
        <div class="box">
          <img src="../../../assets/svg/svg-6.svg" alt="">
          <h3>Regulatory Risk</h3>
          <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit. Error,  </p>
          <i class="fa-solid fa-arrow-right"></i>
        </div>

      </div>
    </div>
      
  </section>
</template>

<script>
export default {
    name:'FirstPMain'
}
</script>

<style lang="scss" scoped>
@import "../../../assets/style-scss/variables.scss";

  p{
    color:#939ca1;
  }
  .services{
    background-color:#eef4ed;
    min-height: 650px;
    padding-top: 50px;
    padding-bottom: 100px;
    .container{
     
      margin: 0 auto;
    
      .section-text{
        position: relative;
       
        h2{
          margin-bottom: 20px;
          font-weight: 900;
          font-size: 40px;
        }
        p{
          width: 750px;
        }
        .btn{
          position: absolute;
          right: 0;
          bottom: 0px;         
        }
      }

      .box-container{
        width: 100%;
        margin-top: 30px;
        display: flex;
        flex-wrap: wrap;
        .box{
          position: relative;
          width: calc(100% /3 - 20px);
          margin: 10px;
          background-color: $colorWhite;
          border-radius: 10px;
          padding: 20px;
          min-height: 180px;

          &:hover .fa-arrow-right{
            background-color:#7cd1d1;
            border-radius: 50%;
            
          }

          h3{
            margin: 10px 0px;
          }
          .fa-arrow-right{
            position: absolute;
            top: 20px;
            right: 20px;
            font-size: 20px;
            color: $colorBlueLagon;
            padding: 10px;
          }
          img{
            width: 30px;
            filter: invert(36%) sepia(19%) saturate(3322%) hue-rotate(142deg) brightness(98%) contrast(98%);
          }
        }
      }
    }
  }
</style>