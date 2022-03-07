<template>
<!-- Sezione con i dati raccolti sul gruppo -->
  <section class="result">
      <div class="top-section">
          <div class="container">
                <div class="title-section">  
                    <h6>WHAT ARE WE DOING</h6>
                    <h2><span class="secondoevidenziatore">Result</span> in numbers</h2>
                </div>
                <nav>
                    <li>
                        <span class="value">128</span>
                        <ul>
                            <li class="category"><a href="#">Certification</a></li>
                        </ul>
                    </li>
                    <li>
                        <span class="value">230</span>
                        <ul>
                            <li class="category"><a href="#">Employees</a></li>
                        </ul>
                    </li>
                    <li>
                        <span class="value">517</span>
                        <ul>
                            <li class="category"><a href="#">Customers</a></li>
                        </ul>
                    </li>
                    <li>
                        <span class="value">94</span>
                        <ul>
                            <li class="category"><a href="#">Countries Served</a></li>
                        </ul>
                    </li>
                </nav>
          </div>
      </div>

      <!-- Sezione con logo dei vari sponsor -->
      <div class="bottom-section">
            <div class="box-container">
                    <div class="box">
                        <img src="../../../assets/img/logo-4.png" alt="">

                    </div>
                    <div class="box">
                        <img src="../../../assets/img/logo-5.png" alt="">

                    </div>
                    <div class="box">
                        <img src="../../../assets/img/logo-1.png" alt="">

                    </div>
                    <div class="box">
                        <img src="../../../assets/img/logo-2.png" alt="">

                    </div>
                    <div class="box">
                        <img src="../../../assets/img/logo-3.png" alt="">

                    </div>
                    <div class="box">
                        <img src="../../../assets/img/logo-4.png" alt="">

                    </div>

            </div>
      </div>

  </section>
</template>

<script>
export default {
    name:'FourthPMain'
}
</script>

<style lang="scss" scoped>
@import "../../../assets/style-scss/variables.scss";
    .container{
        margin: 20px auto;
        text-align: center;
        height: 100%;
    }
  
    .result{
        height: 600px;
        .top-section{
            background-image: url("../../../assets/img/bg-7.jpg");
            background-size: cover;
            background-position: center;
            height: 500px;
            position: relative;

            .title-section{
                padding-top: 100px;
               
                h2{
                    margin: 20px 0;
                    font-weight: 900;
                    font-size: 50px;
                    color:$colorWhite;
                }
            }

            nav{
                display: flex;
                justify-content: center;
                align-items: center;
                width: 100%;
                padding-top: 50px;

                .value{
                    color: $colorBlueLagon;
                    font-size: 30px;
                    font-weight: 600;
                }
                ul{
                    margin: 0 50px;
                    .category{
                        a{
                            font-weight: 600;
                            color:$colorWhite;
                            font-size: 18px;
                        }
                    }
                }
            }
        }
        .bottom-section{
            background-color: $MCcolorShark;
            height: 200px;
            width: 100%;
            display: flex;
            justify-content: center;
        
            .box-container{
                height: 100%;
                width: 70%;
                display: flex;
                flex-wrap: wrap;
                align-items: center;
                justify-content: space-around;
                .box{

                    img{
                       width: 100px;
                       height: 100px;
                       object-fit: contain;
                       filter: brightness(500%);
                    }
                }
            }
        }
    }



</style>