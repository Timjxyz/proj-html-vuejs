<template>
<div class="header-bottom">
    <div class="container">
        <div class="header-nav d-flex">
            <!-- Parte sinista con logo -->
            <div class="logo">
                <img src="../../../assets/img/logo.png" alt="">
            </div>

            <!-- Parte destra con barra di navigazione -->
            <nav>
                <ul>
                    <NavHeader
                        v-for="(navItem, index) in navItems" 
                        :key="index"
                        :nav="navItem.title"
                    />
                    <li>
                        <div class=" btn btn-green btn-hover">
                            <a href="#"> GET IN TOUCH</a>
                         </div>
                    </li> 
                </ul>

            </nav>

        </div>

    </div>
    <!-- Sezione jumbotron -->
    <div class="jumbotron">
        <div class="jumbotron-bg"></div>

        <div class="text-jumbo">
            <h1>Ready <span class="evidenziatore">Team</span></h1>
            <p>No matter what your company needs, we will be ready to assist you in the best possible way.</p>
            <div class=" btn btn-green btn-hover">
              <a href="#"> GET IN TOUCH</a>
            </div>
            <div class=" btn btn-transparent btn-hover">
                <a href="#">READ MORE</a>
            </div>
        </div>
        <div class="select">
            <div class="pipe"></div>
            <div class="pipe pipe-active"></div>
            <div class="pipe"></div>
        </div>
    </div>
    
</div>
  
</template>

<script>
import NavHeader from './NavHeader.vue'

export default {
    name:'HeaderBottom',
    components:{
        NavHeader
    },
    data(){
        return{
            navItems:[
                {
                    "title":"HOME"
                },
                {
                    "title":"SERVICES"
                },
                {
                    "title":"ABOUT"
                },
                {
                    "title":"PROJECTS"
                },
                {
                    "title":"RESULTS"
                }
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../../../assets/style-scss/variables.scss";
    .header-bottom{
        padding-top: 20px;
        background-image: url("../../../assets/img/bg-jumbo.jpg");
        
       
        .container{
            align-items: center;
            justify-content: space-between;
            height: 100%;
            //Regole parte nav
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
                            
                        }
                    }
                }  
            }

        }
        .btn{
            margin-right: 10px;

            a{                  
                text-decoration: none;
            }
        }
        //Regole sezione jumbotron
        .jumbotron{
             position: relative;
            .jumbotron-bg{
               min-height: 635px;
               background-image: url('../../../assets/img/bg-parallax.png');
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
                h1{
                    font-size: 60px;
                    font-weight: 900;
                }

                p{
                    margin-bottom: 30px;
                    color:#939ca1;
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
                .pipe-active{
                    background-color: $colorBlueLagon;
                }
            }

        }
    }


</style>