<template>
<!-- Sezione sulle caratteristiche della compagnia -->
  <section class="company">

    <div class="left-container">
        <!-- Titolo della sezione -->
        <div class="section-text">
            <h6>OBOUT THE NETWORK</h6>
            <h2><span class="secondoevidenziatore">The</span> Company</h2>
            <p>
                For 12 years we have been providing audit and warranty, 
                financial advice, taxes and related service to select clients.
            </p>
            
        </div>
        <!-- Contenitore box certificati -->
        <div class="box-container">
            <!-- Box 1 -->
            <div class="box">
                <i class="fa-solid fa-award"></i>
                <h3>Tradition</h3>
                <p>Lorem ipsum dolor, sit amet consectetur, lorem</p>
                
            </div>
             <!-- Box 2 -->
            <div class="box">
                <i class="fa-solid fa-lock"></i>
                <h3>Security</h3>
                <p>Lorem ipsum dolor, sit amet consectetur, lorem</p>
                
            </div>
             <!-- Box 3 -->
            <div class="box">
                <i class="fa-solid fa-pen-to-square"></i>
                <h3>Certificate</h3>
                <p>Lorem ipsum dolor, sit amet consectetur, lorem</p>
                
            </div>
             <!-- Box 4 -->
            <div class="box">
                <i class="fa-solid fa-graduation-cap"></i>
                <h3>Expertise</h3>
                <p>Lorem ipsum dolor, sit amet consectetur, lorem</p>
                
            </div>
             <!-- Bottoni della sezione -->
            <div class="btn btn-green btn-hover">
                <a href="#"> GET IN TOUCH</a>
            </div>
            <div class="btn btn-transparent btn-hover">
                <a href="#"> READ MORE</a>
            </div>
        </div>

    </div>

    <!-- Parte destra della sezione con immagine di sfondo -->
    <div class="right-container">
        <img src="../../../assets/img/about-4.jpg" alt="">
    </div>

  </section>
</template>

<script>
export default {
    name:'SecondPMain'
}
</script>

<style lang="scss" scoped>
@import "../../../assets/style-scss/variables.scss";
    .company{
        height: 700px;
        background-color:#111117;
        display: flex;
        //Regole parte destra della sezione
        .left-container{
            width: 50%;
            margin-top: 50px;
            
            .section-text{
                width: 65%;
                margin-left: auto;

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
                    margin-right: 30px;
                    margin-top: 30px;
                }

           }
          
        }

        //Regole sull'imagine di sfondo della parte destra della sezione
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