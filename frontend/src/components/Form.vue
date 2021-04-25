<template>
<form>
<div class="grid-container">
<Input Label="Product Name" type="text"  />
<Input Label="Price" type="text"  />
<Input Label="Product Discription" inputId="discribe" SubLabel=" (Optional)" type="textarea"  />
<Input Label="Product Image" SubLabel=" (Optional)" type="file" />
<button @click="addProduct" class="btn"><b>Add Product</b></button>

</div>
</form>

</template>

<script>
import Input from "./Input"

export default {

    name:'Form',
    components:{
      Input
    },
    
}
</script>
<style>
.grid-container {
  display: grid;
  grid-template-columns: auto auto ;
  margin: 0;
  padding: 2rem 1.5rem;
  font: 1rem/1.5 "PT Sans", Arial, sans-serif;
  color: #3d3939;
}
.btn{
  width:fit-content;
  padding: 12px 20px;
  margin: 8px 20px;
  background-color: #39b5e9;
  color:#fff;
  border: 1px solid #fff;
  

}
</style>

