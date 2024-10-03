<script>
    export default {
        props: {
            link: String,
            textodoBotao: String
        }
    }

</script>
<template>
<div >
    <a :href="link">{{textodoBotao}}></a>
</div>

</template>
<style scoped>
    div {
        padding: 10px;
        padding: 20px;
        float: left;

    }
    a{
        color: 000;
        padding: 10px 20px;
        
    }
    a:hover{
        color: white;
        background-color: green;
        padding: 10px 20px;
    }
</style>