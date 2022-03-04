<template>
<!-- Seconda sezione del menù -->
  <section class="company">

    <div class="left-container">
        <!-- Titolo della sezione -->
        <div class="section-text">
            <h6>OBOUT THE NETWORK</h6>
            <h2>The Company</h2>
            <p>
                For 12 years we have been providing audit and warranty, 
                financial advice, taxes and related service to select clients.
            </p>
            
        </div>
        <!-- Contenitore box item -->
        <div class="box-container">
            <div class="box">
                <i class="fa-solid fa-award"></i>
                <h3>Tradition</h3>
                <p>Lorem ipsum dolor, sit amet consectetur, lorem</p>
                
            </div>
            <div class="box">
                <i class="fa-solid fa-lock"></i>
                <h3>Security</h3>
                <p>Lorem ipsum dolor, sit amet consectetur, lorem</p>
                
            </div>
            <div class="box">
                <i class="fa-solid fa-pen-to-square"></i>
                <h3>Certificate</h3>
                <p>Lorem ipsum dolor, sit amet consectetur, lorem</p>
                
            </div>
            <div class="box">
                <i class="fa-solid fa-graduation-cap"></i>
                <h3>Expertise</h3>
                <p>Lorem ipsum dolor, sit amet consectetur, lorem</p>
                
            </div>
            <div class="btn">
                <a href="#"> GET IN TOUCH</a>
            </div>
            <div class="btn">
                <a href="#"> READ MORE</a>
            </div>
        </div>

    </div>
    <div class="right-container">
        <img src="../../assets/img/about-4.jpg" alt="">
    </div>

  </section>
</template>

<script>
export default {
    name:'SecondPMain'
}
</script>

<style lang="scss" scoped>
@import "../../assets/style-scss/variables.scss";
    .company{
        height: 700px;
        background-color: $MCcolorShark;
        display: flex;

        .left-container{
            width: 50%;
            margin-top: 50px;
            
            .section-text{
                width: 65%;
                margin-left: auto;

                h6{
                    color: $colorBlueLagon;
                    margin-bottom: 20px;
                }
                h2{
                    color:$colorWhite;
                    font-weight: 900;
                    font-size: 40px;
                    margin-bottom: 20px;
                }
                p{
                    color:$MCcolorGrayNurse;
                }
            }

             .box-container{
                width: 65%;
                margin-left: auto;
                margin-top: 30px;
                display: flex;
                flex-wrap: wrap;
                .box{
                    position: relative;
                    width: calc(100% /2 - 40px);
                    margin: 20px;
                    

                    h3{
                        padding-left: 10px;
                        color:$colorWhite;
                        margin: 10px 0px;
                        display: inline-block;
                    }
                    p{
                        color:$colorGravel;
                    }
                    .fa-solid{
                        font-size: 30px;
                        color: $colorBlueLagon;
                    }
               }

               .btn{
                     margin-right: 10px;
                     display: inline-block;
                     margin-top: 30px;
                }

               a{
                    text-decoration: none;
                    color: #fff;
                    padding: 5px 14px;
                    border-radius: 2px;
                    background-color: $colorBlueLagon;
                    margin-bottom: 10px;
               }
           }
          
        }
        .right-container{
            width:50%;
            
            img{
                width: 100%;
                height: 100%;
                object-fit: cover;
            }
        }
    }

</style>