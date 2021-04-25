<template>
 
     <Form/>
     <ProductList :Items="Items"/>

 
</template>

<script>
// @ is an alias to /src
import Form from '@/components/Form.vue'
import ProductList from '@/components/ProductList.vue'
export default {
  name: 'Manage',
  components: {
    Form,
    ProductList,
  },
  data() {
        return{
         Items: []

        }
           
    },
    created()
    {
         this.Items =[
          {
            id:1,
             title:"This is Product",
             discription:"This is dicription",
             price:100
          },
         {
           id:2,
           title:"This is Product 2",
            discription:"This is dicription 2",
            price:200
         },
         {
           id:3,
           title:"This is Product 3",
            discription:"This is dicription 3",
            price:300
         },
         ]
    }
}
</script>
