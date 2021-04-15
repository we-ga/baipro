<template>
  <div id="nav" style="overflow: hidden; display: inline-block;">
       <img style="width:100px"  :src="image" />
          <a style="font-size: 30px; margin-right:80px; border-radius: 4px;opacity:0.8">e-Student</a>
    <router-link to="/">Home</router-link> |
    <router-link :to="{ name: 'Student' }">Student List
    </router-link>
    <router-link :to="{ name: 'Achievements' }">Chart</router-link>
    <router-link :to="{ name: 'Grades' }">Grades</router-link>
  
  </div>
  

  <router-view />
</template>
<script>

import image from "./assets/logo.png"

export default {
data: function () {
  return {
    image: image
  }
},

};
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
 
  
}

#nav {

display: inline-block;
padding:30px;
padding-right: 100px;

}

#nav a {
  font-size: 20px;
  font-weight: bold;
  color: #2c3e50;
  text-decoration: none;
  padding: 10px;
  border-radius: 4px;
}

#nav a.router-link-exact-active {
  color: white;
  background-color: crimson;
}
button {
  margin: 0 10px;
  padding: 10px;
  border: none;
  border-radius: 4px;
}





</style>


