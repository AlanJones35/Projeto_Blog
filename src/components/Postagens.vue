<script>
export default{
    name: "Postagens",
    props: {
        imagem: String,
        titulo: String,
        mensagem: String,
        autor: String
    }
}
</script>

<template>  
    <div id="container">
        <img v-if="imagem" :src="imagem" alt="sem imagem">
        <h1 class="tit">{{ titulo }}</h1>
        <p class="men">{{ mensagem }}</p>
        <br>
        <span class="aut">{{ autor }}</span>
    </div>
</template>

<style scoped>
    #container{
    position: relative;
    background-color: rgb(187, 181, 181);
    width: 1140px;
    height: 1100px;
    }
    
    .tit{
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    font-size: 50px;
    color: black;
    display: flex;
    text-align: justify;
    margin-left: 10px;
    margin-right: 10px;

    }
    .men{
    font-size: 25px;
    color: black;
    display: flex;
    text-align: justify;
    margin-left: 10px;
    margin-right: 10px;
    }
    
    .aut{
    font-family: Georgia, 'Lucida Sans', 'Times', 'serif';
    font-size: 20px;
    color: black;
    display: flex;
    margin-left: 10px
    }
</style>