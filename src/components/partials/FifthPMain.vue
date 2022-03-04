<template>
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
                <form>
                    <input type="text" placeholder="Name">
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
                       <option value="">More Info</option>
                       <option value="">More Info</option>
                       <option value="">More Info</option>
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
        margin-top: 100px;
        height: 700px;
       
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
                    color:$MCcolorGrayNurse;
                    border-radius: 5px;
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
            
            img{
                width: 100%;
                height: 100%;
                object-fit: cover;
            }
        }
    }

</style>