<template>
    <!-- Componente per rendere dinamiche le voci nella barra di navigazione -->
    <li>
        <a class="link" href="#">{{nav}}</a>
    </li>

</template>

<script>
export default {
    name:"NavHeader",
    props: {
        "nav": String,
        
    },
}
</script>

<style lang="scss" scoped>
@import "../../../assets/style-scss/variables.scss";

li{
    margin: 0 10px;
    display: inline-block;
    .link{
        text-decoration: none;
        color: $ColorWoodSmoke;
    }
    
}


</style>