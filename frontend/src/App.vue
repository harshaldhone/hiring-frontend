<template>
 
  <div id="nav">
    <div class="logo">
      <img src="./assets/logo_5e006325d2b351577083685.png" alt="">
    </div>
    <router-link to="/">Home</router-link> 
    <router-link to="/manage-product">Manage Products</router-link>
    
  </div>
  <router-view/>
</template>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}

#nav {
  padding: 30px;
  display: flex;
  justify-content:flex-start;
  align-items: center;
  background-color: #fff;
}

#nav a {
  font-weight: bold;
  color: #2c3e50;
  margin: 0px 20px 0px 0px;
}

#nav a.router-link-exact-active {
  color: #42b983;
}
.logo{
  margin-right: 50px;
}
</style>
