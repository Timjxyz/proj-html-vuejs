<template>
  <section class="project">
      <div class="container">
          <!-- Titolo della sezione -->
          <div class="section-title">
            <h6>WE DO MORE FORE EVERYONE</h6>
            <h2>Actions & Projects</h2>

          </div>
            <!-- Barra di navigazione all'internzo della sezione -->
          <nav>
              <ul>
                  <li><a href="#">ALL</a></li>
                  <li><a href="#">INSTITUTIONAL</a></li>
                  <li><a href="#">SOCIAL</a></li>
                  <li><a href="#">EVENTS</a></li>
                  <li><a href="#">INNOVATION</a></li>
                  <li><a href="#">ENVIRONMENT</a></li>
                  <li><a href="#">TECHNOLOGY</a></li>
              </ul>
          </nav>

            <!-- Conenitore box -->
          <div class="box-container">
                <div class="box">
                    <img src="../../assets/img/project-1.jpg" alt="">
                    <h3>Academic professional program in social media</h3>
                </div>
                <div class="box">
                    <img src="../../assets/img/project-2.jpg" alt="">
                    <h3>Presidet's speech at the annual meeting</h3>
                </div>
                <div class="box">
                    <img src="../../assets/img/project-3.jpg" alt="">
                    <h3>International business trip in Shanghai</h3>
                </div>
                <div class="box">
                    <img src="../../assets/img/project-4.jpg" alt="">
                    <h3>Technology workshop whith education theme</h3>
                </div>
                <div class="box">
                    <img src="../../assets/img/project-5.jpg" alt="">
                    <h3>Donation of clothes and food the partner NGO</h3>
                </div>
                <div class="box">
                    <img src="../../assets/img/project-6.jpg" alt="">
                    <h3>Confraternization of the procurement team</h3>
                </div>
          </div>
      </div>
  </section>
</template>

<script>
export default {
    name:'ThirdPMain'
}
</script>

<style lang="scss" scoped>
@import "../../assets/style-scss/variables.scss";
    .project{
        min-height: 600px;
        margin-top: 100px;
        .container{
            width: 70%;
            margin:auto;
            text-align: center;
            .section-title{
                margin-bottom: 20px;
                h6{
                    margin-bottom: 20px;
                    color: $colorBlueLagon;
                }
            }
            nav{
                ul{
                    li{
                        display: inline-block;
                        list-style: none;
                        a{
                           margin: 10px 20px;
                           color: $colorPumice;
                        }
                    }
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
                    overflow: hidden;
                  
                    h3{
                        margin: 10px 0px;
                        position: absolute;
                        bottom: 10px;
                        text-align: center;
                        color: $colorWhite;
                        font-size: 24px;
                    }
                    img{
                       width: 100%;
                       height: 100%;
                       object-fit: cover;
                    }
                }
            }
        }
    }

</style>