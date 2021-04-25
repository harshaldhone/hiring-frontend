<template>
    <ul>
        <li>
            <span><img src="https://source.unsplash.com/random" alt="logo"></span>
            <span>{{Item.title}}</span>
            <span>{{Item.discription}}</span>
            <span>{{Item.price}}</span>
            <span>Remove</span>
        </li>
    </ul>
</template>
<script>
export default {
    name: 'ProductListItem',
    props:{
        Item:Object,
    },
    
}
</script>
<style >
ul{
    margin:0px;
}
ul li{
   
    display: flex;
    align-items:center;
    text-align: left;
}
ul li span:nth-child(1){
    width: 100px;
}
ul li span:nth-child(2){
    width: 200px;
}
ul li span:nth-child(3){
    width: 200px;
}
ul li span:nth-child(4){
    width: 200px;

}
ul li span:nth-child(5){
    width: 200px;
    color: rgb(253, 5, 5)
}
img{
    width:50px;
    height: 50px;
}
</style>