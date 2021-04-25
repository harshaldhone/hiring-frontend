<template>
    <div class="container">
        <hr class="line">
            <div>
            <ul>
                <li>
                    <span></span>
                    <span><b>Name</b></span>
                    <span><b>Description</b></span>
                    <span><b>Price</b></span>
                </li>
            </ul>
            </div>
        <hr class="line">
        <div :key="Item.id" v-for="Item in Items">
            <ProductListItem :Item="Item"/>
            <hr class="thin-line">
        </div>
        
    </div>
</template>
<script>
import ProductListItem from "./ProductListItem"
export default {
    name:'ProductList',
    components: {
        ProductListItem,
    },
    props: {
        Items:Array
    }
    
}
</script>
<style >
.container{
    margin: 0;
    
}
.line{
    opacity: 90;
    border: 1px solid  rgb(180, 176, 176);
    margin: 0rem 2rem;
}
.thin-line{
    opacity: 10;
    border: 1px solid #ccc;
    margin: 0rem 2rem;
}
ul{
    margin:10px;
    
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
</style>