<template>
    <div class="jumbotron">
        <Card/>
    </div>
    
    
</template>
<script>
import Card from "./Card"
export default {
    name:'Cards',
    props:{
        title:String
    },
    components:{
        Card
    }
}

</script>

<style>
.jumbotron{
    
    background-color: antiquewhite;
    display:grid;
    margin: 5% 10%;
    grid-template-columns: repeat(3,1fr);
    gap:20px;
    font-family: sans-serif;
}
</style>
