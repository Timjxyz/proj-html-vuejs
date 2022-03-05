<template>

<!-- Sezione con il form e contatti -->
  <section class="form">
      
    <div class="left-container">
        <!-- Titolo della sezione -->
        <div class="section-text">
            <h6>SEND A MESSAGE</h6>
            <h2>Get in Thouch</h2>
            <p>
                We will respond to your message as possible.
            </p>
            
        </div>
        <!-- Contenitore box item -->
        <div class="box-container">
            <div class="box">
                <form class="name-form">
                    <input type="text" placeholder="Name">
                    <img src="../../assets/img/image (1).png" alt="">
                </form>
            </div>
            <div class="box">
                 <form>
                    <input type="mail" placeholder="Email">
                </form>
                
            </div>
            <div class="box">
               <form>
                    <input type="number" placeholder="Phone">
                </form>
                
            </div>
            <div class="box">
               <form>
                    <select >
                       <option value="">More Info</option>
                       <option value="">To Sign Up</option>
                       <option value="">Other</option>
                    </select>
                </form>
                
            </div>
            <div class="text-area">
                <textarea  rows="10"></textarea>
            </div>
            <div class="btn">
                <a href="#"> SEND</a>
            </div>
        </div>

    </div>
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
                    <div class="btn">
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
    @import "../../assets/style-scss/variables.scss";
    .form{
        margin: 100px 0px;
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
                    color:$ColorWoodSmoke;
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
                    color:$MCcolorGrayNurse;
                    padding: 10px;
                    border-radius: 5px;
                }
                select{
                    padding: 10px;
                    width: 90%;
                    background-color:#ececec; 
                    border-radius: 5px;
                    option{
                        color:$MCcolorGrayNurse;
                    }
                }
                .text-area{
                    width: 100%;
                 
                    textarea{
                        background-color:#ececec;
                        width: 95%;
                        color:$MCcolorGrayNurse;
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
                                text-decoration: none;
                                padding: 5px 30px;
                                border-radius: 2px;
                                border: 1px solid  $colorBlueLagon;
                                margin-bottom: 10px;

                            }
                        }
                    }
                }
            }
            
           
        }
    }

</style>