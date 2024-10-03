<script>
import Botao from       "./Botao.vue"
import logo from        "./imgs/favicon.png"
export default{
    props:{
        logotipo: String,
        textodoBotao: String,
        link: String
    },
    data() {
        return {            
            logo             
        };   
    },
    components: {
        Botao,
        logo 
    }
}
</script>

<template>
    <div>
        <img id="log":src="logo">
        
        <Botao textodoBotao="Login/Logout" link="./AreaPostagem.vue" />
        <Botao textodoBotao="Home" link="./AreaPostagem.vue" />
        <Botao textodoBotao="Postagem" link="./AreaPostagem.vue" />
        <Botao textodoBotao="Inscreva-se" link="./AreaPostagem.vue" />    
    </div>  
</template>

<style>
    #log{
        width: 250px;
        margin-left: 5px
    }
    #btn{
        font-size: 15px;
        color: aqua;
    }   
    #container{

    position: relative;
    background-color: rgb(187, 181, 181);
    width: 140px;
    height: 100px;
    }
</style>