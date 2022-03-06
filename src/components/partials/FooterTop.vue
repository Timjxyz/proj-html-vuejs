<template>

<!-- PARTE SUPERIORE DEL FOOTER -->
    <div class="footer-top">

        <!-- Contenitore del footer -->
        <div class="container">

            <div class="box">
                <div class="logo-footer">
                    <img src="../../assets/svg/svg-7.svg" alt="">
                </div>
                <p>A Functional HTML Template for Corporate & Business</p>
                <nav class="info-nav info-contacts">
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
                            <div class="btn btn-transparent btn-hover">
                                <a href="#"> GET IN TOUCH</a>
                            </div>
                        </li>
                    </ul>
                </nav>
            </div>
            <div class="box list">
                <h2>About</h2>
                <nav class="info-nav">
                    <ul>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#"> The Company</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#"> Institutional</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#"> Social & Events</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#"> Innovation</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#"> Enviroment</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#"> Technology</a>
                        </li>
                    </ul>
                </nav>
            </div>
            <div class="box list">
                <h2>Services</h2>
                <nav class="info-nav">
                    <ul>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#">Audit & Assurance</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#">Financial Advisory</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#">Analytics M&A</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#">Middle Marketing</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#">Legal Consulting</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#">Regular Risk</a>
                        </li>
                    </ul>
                </nav>
            </div>  
            <div class="box list">
                <h2>Support</h2>
                <nav class="info-nav">
                    <ul>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#">Responsibility</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#">Terms of Use</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#">About Cookies</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#">Privacy Policy</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#">Accessibility</a>
                        </li>
                        <li>
                            <i class="fa-solid fa-angle-right"></i>
                            <a href="#">Information</a>
                        </li>
                    </ul>
                </nav>
            </div>    
            
        </div>

    </div>
</template>

<script>
export default {
    name:'FooterTop',
    
}
</script>

<style lang="scss" scoped>
@import "../../assets/style-scss/variables.scss";
    .footer-top{
        padding-top: 100px;
        min-height: 500px;
        background-color: $ColorWoodSmoke;

        .container{
            display: flex;
            .box{
                margin-top: 100px;
                width: calc(100% / 4 - 40px);
                margin: 20px;
                
                &.list{
                    background-color:#19191f;
                    padding: 40px;
                    border-radius: 10px;

                }
                
                h2{
                    color:$colorWhite;
                }

                img{
                    width: 150px;
                    margin-bottom: 20px;
                }
                p{
                    color: $colorGravel;
                }
                .info-contacts{
                    li{
                        padding: 5px 0px;
                    }
                }
                .info-nav{
                     
                    ul{
                        li{
                            color: $colorGravel;
                            list-style: none;
                            margin: 10px 0px;
                            .fa-solid{
                                font-size: 14px;
                                margin-right: 5px; 
                            }
                            a{
                                color: $colorGravel;
                            }

                            .btn{
                                margin-right: 10px;
                                display: inline-block;
                                margin-top: 30px;
                              
                            }
                        }
                    }
                }
            }
        }

    }

</style>