<template>
        <div class="card">
            <div class="card__image">
                <img src="../assets/logo.png" alt="Avatar" style="width:100%">
            </div>
            
            <div class="card__content">
                <p>{{productname}}</p>
                <b>{{price}}:-</b>
            </div>
        </div>
</template>

<script>
export default {
    name:'Card',
    data(){
        return{
            productname:"Television set gdhad asdvagshdvha ",
            price:100,
        }
        
    }
}

</script>
<style scoped>
.card {
  /* Add shadows to create the "card" effect */
  box-shadow: 0 4px 8px 0 rgba(0,0,0,0.2);
  transition: 0.3s;
  
}

.card__image{
    width: 100%;
    display:block;
    
}
.card__image > img{
    height:300px;
}


/* On mouse-over, add a deeper shadow */
.card:hover {
  box-shadow: 0 8px 16px 0 rgba(0,0,0,0.2);
}

/*  some padding inside the card container */
.card__content {
  padding: 16px;
  display:flex;
  justify-content:space-between;
  
  font-size: 1.5em;
  background:#fafafa;
  text-align: left;
  align-items:center;
  
}
.card__content>p{

    margin: 0px 0px;
    
}


</style>