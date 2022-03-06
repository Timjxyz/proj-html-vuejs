<template>
  <section class="project">
      <div class="container">
          <!-- Titolo della sezione -->
          <div class="section-title">
            <h6>WE DO MORE FORE EVERYONE</h6>
            <h2>Actions & <span class="evidenziatore">Projects</span></h2>

          </div>
            <!-- Barra di navigazione all'internzo della sezione -->
          <nav>
              <ul>
                  <li><a href="#"><span class="evidenziatore">ALL</span></a></li>
                  <li><a href="#">INSTITUTIONAL</a></li>
                  <li><a href="#">SOCIAL</a></li>
                  <li><a href="#">EVENTS</a></li>
                  <li><a href="#">INNOVATION</a></li>
                  <li><a href="#">ENVIRONMENT</a></li>
                  <li><a href="#">TECHNOLOGY</a></li>
              </ul>
          </nav>

            <!-- Conenitore box con immagini-->
          <div class="box-container">
              <!-- Box 1 -->
                <div class="box">
                    <img src="../../assets/img/project-1.jpg" alt="">
                    <a href="#">
                       <i class="fa-solid fa-arrow-right"></i>
                    </a>
                    <div class="text-img">
                       <h3>Academic professional program in social media</h3>
                       <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                    </div>
                </div>
                 <!-- Box 2 -->
                <div class="box">
                    <img src="../../assets/img/project-2.jpg" alt="">
                    <a href="#">
                       <i class="fa-solid fa-arrow-right"></i>
                    </a>
                    <div class="text-img">
                       <h3>Presidet's speech at the annual meeting</h3>
                       <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                    </div>
                </div>
                 <!-- Box 3 -->
                <div class="box">
                    <img src="../../assets/img/project-3.jpg" alt="">
                    <a href="#">
                       <i class="fa-solid fa-arrow-right"></i>
                    </a>
                    <div class="text-img">
                        <h3>International business trip in Shanghai</h3>
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                    </div>
                </div>
                 <!-- Box 4 -->
                <div class="box">
                    <img src="../../assets/img/project-4.jpg" alt="">
                    <a href="#">
                       <i class="fa-solid fa-arrow-right"></i>
                    </a>
                    <div class="text-img">
                       <h3>Technology workshop whith education theme</h3>
                       <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                    </div>
                </div>
                 <!-- Box 5 -->
                <div class="box">
                    <img src="../../assets/img/project-5.jpg" alt="">
                    <a href="#">
                       <i class="fa-solid fa-arrow-right"></i>
                    </a>
                    <div class="text-img">
                      <h3>Donation of clothes and food the partner NGO</h3>
                      <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                    </div>
                </div>
                <!-- Box 6 -->
                <div class="box">
                    <img src="../../assets/img/project-6.jpg" alt="">
                    <a href="#">
                       <i class="fa-solid fa-arrow-right"></i>
                    </a>
                    <div class="text-img">
                        <h3>Confraternization of the procurement team</h3>
                        <p>Lorem ipsum dolor, sit amet consectetur adipisicing elit.</p>
                    </div>
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
            text-align: center;
            .section-title{
                margin-bottom: 20px;
                h6{
                    margin-bottom: 20px;
                    color: $colorBlueLagon;
                }
                h2{
                    font-weight: 800;
                    font-size: 30px;
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
                           .evidenziatore{
                               padding: 10px;
                           }
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
                    &:hover .text-img p{
                        display: block;
                    }

                    &:hover img{
                        filter: blur(2px);
                        
                    }
                    &:hover .fa-arrow-right{
                        display: block;
                    }
                    .fa-arrow-right{
                        position: absolute;
                        color: $colorWhite;
                        top: 20px;
                        right: 20px;
                        font-size: 24px;
                        display: none;
                    }

                    .text-img{
                        margin: 10px 0px;
                        position: absolute;
                        bottom: 10px;
                        text-align: center;
                        color: $colorWhite;
                        font-size: 20px;           

                        p{
                           display: none;
                            
                        }
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