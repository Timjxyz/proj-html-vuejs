<template>

<!-- Componente superiore del header -->

  <div class="header-top">
      <div class="container d-flex">
          <!-- Parte sinistra del nav con orari e giorni di apertura -->
          <div class="time-tables">
              <i class="fa-solid fa-clock"></i>
              <span>Open Hours: Mon - Sat - 9:00 - 18:00</span>
          </div>

          <!-- Parte destra del nav con i vari contatti -->
          <div class="contacts d-flex">
              <!-- Link al numero di telefono -->
                <span  class="phone-number">
                    <i class="fa-solid fa-phone"></i>
                    <span>
                            <a href="#">
                                +1(305) 1234-5678
                            </a> 
                    </span>

                </span>
                <!-- Link alla mail -->
                <span class="mail">
                        <i class="fa-solid fa-envelope"></i>
                        <span>
                            <a href="#">
                                hello@example.com
                            </a>
                        </span>
                </span>
                <!-- Collegamento ai vari social -->
                <span class="social">
                    <a href="#"><i class="fa-brands fa-facebook-f"></i></a>
                    <a href="#"><i class="fa-brands fa-twitter"></i></a>
                    <a href="#"><i class="fa-brands fa-linkedin-in"></i></a>
                </span>
          </div>

      </div>

  </div>
</template>

<script>
export default {
    name:'HederTop'

}
</script>

<style lang="scss" scoped>
@import "../../assets/style-scss/variables.scss";


    .header-top{
        height: 50px;
        background-color:#21333e;

        a{
            color: $MCcolorGrayNurse;
            text-decoration: none;
        }

        .container{
            align-items: center;
            justify-content: space-between;
            height: 100%;
            color: $MCcolorGrayNurse;

            .time-tables{
               .fa-clock{
                   margin-right: 10px;
               }
            }

            .contacts{
                justify-content: space-around;
                .mail{
                    margin-left: 20px;
                }

                .social{
                    i{margin:0 15px}
                }
            }

        }
        
    }

</style>