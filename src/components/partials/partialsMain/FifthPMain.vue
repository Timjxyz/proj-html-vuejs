<template>

<!-- Sezione con il form e contatti -->
  <section class="form">
      
    <div class="left-container">
        <!-- Titolo della sezione -->
        <div class="section-text">
            <h6>SEND A MESSAGE</h6>
            <h2>Get in <span class="evidenziatore">Thouch</span></h2>
            <p>
                We will respond to your message as possible.
            </p>
            
        </div>
        <!-- Contenitore box item  e form-->
        <div class="box-container">
            <div class="box">
                <form class="name-form">
                    <input type="text" placeholder="Name">
                    <img src="../../../assets/img/image (1).png" alt="">
                </form>
            </div>
            <div class="box">
                 <form>
                    <input type="mail" placeholder="Email">
                </form>
                
            </div>
            <div class="box">
               <form>
                    <input type="text" placeholder="Phone">
                </form>
                
            </div>
            <div class="box">
               <form>
                    <select >
                       <option value="moreInfo">More Info</option>
                       <option value="toSignUp">To Sign Up</option>
                       <option value="support">Support</option>
                       <option value="other">Other</option>
                    </select>
                </form>
                
            </div>
            <div class="text-area">
                <textarea  rows="10"></textarea>
            </div>
            <div class="btn btn-green">
                <a href="#"> SEND</a>
            </div>
        </div>

    </div>

    <!-- Parte destra della sezione con lista contatti -->
    <div class="right-container">
        <div class="contact-text">
            <h3>Example Inc.</h3>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. </p>
            <p> Magnam rem culpa quia earum error obcaecati rerum.</p>
        </div>

        <nav class="info-contacts">
            <ul>
                <li>
                     <i class="fa-solid fa-phone"></i>
                     <a href="#">
                        +1(305) 1234-5678
                    </a> 
                </li>
                <li>
                    <i class="fa-solid fa-envelope"></i>
                    <a href="#">
                        hello@example.com
                    </a>
                </li>
                <li>
                     <i class="fa-solid fa-location-dot"></i>
                     <a href="#">
                        Main Avenue, 987
                    </a> 
                </li>

                <li>
                    <div class="btn btn-transparent">
                        <a href="#"> VIEW MAP</a>
                    </div>
                </li>
            </ul>
        </nav>
    </div>
  </section>
</template>

<script>
export default {
    name:'FifthPMain'
}
</script>

<style scoped lang="scss">
    @import "../../../assets/style-scss/variables.scss";
    .form{
        margin: 100px 0px;
        display: flex;

        .left-container{
            width: 50%;
            margin-top: 50px;
            
            //Parte superiore sx con regole titolo della sezione e testo
            .section-text{
                width: 65%;
                margin-left: auto;

                h2{
                    color:$ColorWoodSmoke;
                    font-weight: 900;
                    font-size: 40px;
                    margin-bottom: 20px;
                }
                p{
                    color:#939ca1;
                }
            }

            //Parte sx della sezione con regole del form
             .box-container{
                width: 65%;
                margin-left: auto;
                margin-top: 30px;
                display: flex;
                flex-wrap: wrap;

                .name-form{
                    position: relative;
                    img{
                        position: absolute;
                        top: 50%;
                        right: 30px;
                        transform: translateY(-50%);
                    }
                }
                input{
                    width: 90%;
                    background-color:#ececec;
                    color:$colorPumice;
                    padding: 10px;
                    border-radius: 5px;
                }
                select{
                    padding: 10px;
                    width: 90%;
                    background-color:#ececec; 
                    border-radius: 5px;
                    option{
                        color:$colorPumice;
                    }
                }
                .text-area{
                    width: 100%;
                 
                    textarea{
                        background-color:#ececec;
                        width: 95%;
                        color:$colorPumice;
                        border-radius: 5px;
                        
                    }
                }
                .box{
                    position: relative;
                    width: calc(100% /2 );
                    margin-bottom: 10px;
                    
                    

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
                   
                padding: 5px 14px;

               }
           }
          
        }

        // Regole parte destra della sezione con lista contatti
        .right-container{
            width:50%;
            margin-top: 50px;
            padding-left: 50px;

            .contact-text{
                width: 48%;

                p{
                    margin: 20px 0px;
                }
            }

            .info-contacts{
                ul{
                    li{
                        color: $colorBlueLagon;
                        list-style: none;
                        margin: 10px 0px;
                        .fa-solid{
                            font-size: 20px;
                            margin-right: 10px;
                            padding: 10px;
                            height: 40px;
                            width: 40px;
                            vertical-align: middle;
                            text-align: center;
                            background-color: rgba(3,132,132,0.2);
                            border-radius: 50%;
                        }
                        a{
                            color: $colorBlueLagon;
                        }

                        .btn{
                            margin-right: 10px;
                            display: inline-block;
                            margin-top: 30px;
                            a{                                
                                padding: 5px 16px;
                            }
                        }
                    }
                }
            }
            
           
        }
    }

</style>