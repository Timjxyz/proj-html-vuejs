<template>
<div class="header-bottom">
    <div class="container">
        <div class="header-nav d-flex">
            <!-- Parte sinista con logo -->
            <div class="logo">
                <img src="../../assets/img/logo.png" alt="">
            </div>

            <!-- Parte destra con barra di navigazione -->
            <nav>
                <ul>
                    <li>
                        <a href="#">HOME</a>
                    </li>
                    <li>
                        <a href="#">SERVICES</a>
                    </li>
                    <li>
                        <a href="#">ABOUT</a>
                    </li>
                    <li>
                        <a href="#">PROJECTS</a>
                    </li>
                    <li>
                        <a href="#">RESULTS</a>
                    </li>
                    <li>
                        <a href="#">GET IN TOUCH</a>
                    </li>
                </ul>

            </nav>

        </div>

    </div>

    <div class="jumbotron">
        <div class="jumbotron-bg"></div>

        <div class="text-jumbo">
            <h1>Ready Team</h1>
            <p>No matter what your company needs, we will be ready to assist you in the best possible way.</p>
            <div class="btn">
              <a href="#"> GET IN TOUCH</a>
            </div>
            <div class="btn">
                <a href="#">READ MORE</a>
            </div>
        </div>
        <div class="select">
            <div class="pipe"></div>
            <div class="pipe"></div>
            <div class="pipe"></div>
        </div>
    </div>
    
</div>
  
</template>

<script>
export default {
    name:'HeaderBottom'
}
</script>

<style lang="scss" scoped>
@import "../../assets/style-scss/variables.scss";
    .header-bottom{
        padding-top: 20px;
       
        .container{
            margin: auto;
            width: 70%;
            align-items: center;
            justify-content: space-between;
            height: 100%;

            .header-nav{
                align-items: center;
                justify-content: space-between;
                .logo{
                    img{
                        height: 50px;
                    }
                }
    
                nav{
                    ul{
                        li{
                            margin: 0 20px;
                            display: inline-block;
                            a{
                                text-decoration: none;
                                color: $ColorWoodSmoke;
                            }
                            
                        }
                    }
                }
                
            }

        }
        .jumbotron{
             position: relative;
            .jumbotron-bg{
               min-height: 635px;
               background-image: url('../../assets/img/bg-parallax.png');
               background-size: cover;
               background-position: center;
               margin: 0px  50px;
            }
            .text-jumbo{
                position: absolute;
                left: 50%;
                top: 50%;
                transform: translate(-50%, -50%);
                text-align: center;
                width: 340px;

                p{
                    margin-bottom: 30px;
                }
                .btn{
                     margin-right: 10px;
                     display: inline-block;
                }

                a{
                    color: #fff;
                    text-decoration: none;
                    padding: 12px;
                    border-radius: 4px;
                    background-color: #038484;
                   
                }
            }
            .select{
                position: absolute;
                right: 25px;
                top: 50%;
                transform: translateY(-50%);

                .pipe{
                    margin-bottom: 10px;
                    height: 45px;
                    width: 10px;
                    border: 1px solid $colorBlueLagon;
                    border-radius: 50px;
                }
            }

        }
    }


</style>