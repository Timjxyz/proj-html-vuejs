<template>

<!-- PARTE SUPERIORE DEL FOOTER -->
    <div class="footer-top">

        <!-- Contenitore del footer -->
        <div class="container">
            <!-- Box con dati di contatto -->
            <div class="box">
                <div class="logo-footer">
                    <img src="../../../assets/svg/svg-7.svg" alt="">
                </div>
                <p>A Functional HTML Template for Corporate & Business</p>

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
                            <div class="btn btn-transparent btn-hover">
                                <a href="#"> GET IN TOUCH</a>
                            </div>
                        </li>
                    </ul>
                </nav>
            </div>

            <!-- Lista dinamica del nav -->
            <NavFooter title="About" :items="boxAbout"/>
            <NavFooter title="Services" :items="boxServices"/>
            <NavFooter title="Support" :items="boxSupport"/>
            
            
        </div>

    </div>
</template>

<script>
import NavFooter from './NavFooter.vue'
export default {
    name:'FooterTop',
    components:{
        NavFooter
    },
    data(){
        return{
            boxAbout:[
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"The Company",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Institutional",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Social & Events",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Innovation",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Enviroment",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Technology",
                },
               
            ],
            boxServices:[
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Audit & Assurance",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Financial Advisory",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Analytics M&A",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Middle Marketing",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Legal Consulting",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Regular Risk",
                },
               
            ],
            boxSupport:[
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Responsibility",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Terms of Use",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Social & Events",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Privacy Policy",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Accessibility",
                },
                {
                    "icon":"fa-solid fa-angle-right",
                    "text":"Information",
                },
               
            ]
        }
    }
    
}
</script>

<style lang="scss" scoped>
@import "../../../assets/style-scss/variables.scss";
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

                img{
                    width: 150px;
                    margin-bottom: 20px;
                }
                p{
                    color: $colorGravel;
                }

                .info-contacts{
                     
                    ul{
                        li{
                            color: $colorGravel;
                            list-style: none;
                            margin: 10px 0px;
                            padding: 5px 0px;
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