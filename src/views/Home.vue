<template>
  
  <div class = "home">
    
    <HomeHeader> </HomeHeader>
    
    <FeaturedProducts> </FeaturedProducts>
    
    <About> </About>
  
  </div>

</template>

<script>

import HomeHeader from "../components/HomeHeader";

import FeaturedProducts from "../components/FeaturedProducts";

import About from "../components/About";

export default {name: "home", components: {HomeHeader, FeaturedProducts, About} };

</script>

<style lang = "scss" >

section {background-color: whitesmoke;}

nav {background-color: aquamarine;}

</style>