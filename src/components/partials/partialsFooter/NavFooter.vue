<template>
<!-- Componente per rendere dinamico il nav del footer -->
  <div class="box list">
                <h2>{{title}}</h2>
                <nav class="info-nav">
                    <ul>
                        <li v-for="(item,index) in items" :key="index">
                            <i :class="item.icon"></i>
                            <a href="#">{{item.text}}</a>
                        </li>
                    </ul>
                </nav>
            </div>  
</template>

<script>
export default {
    name:"NavFooter",
    props:{
        'title':String,
        'items':Array
    }
}
</script>

<style lang="scss" scoped>
@import "../../../assets/style-scss/variables.scss";
h2{
    color:$colorWhite;
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

        }
    }
}

</style>