<template>

  <div class = "register"> 
    
     <nav class = "sticky NavGrid-container">
    
      <div class = "NavGrid-item">
    
        <ul class = "navbar">
    
          <li> <router-link to = "/"> Home </router-link> </li>
          
          <li> <router-link to = "/register"> Contacta con Nosotros </router-link>  </li>
        
        </ul>
      
      </div>
    
    </nav>
    
    <hr/>

    <Contact> </Contact>
    
    <About> </About>

  </div> 
  
</template>

<script>

import About from "../components/About";

import Contact from "../components/Contact";

export default {
  
  name: "register",

  components: {Contact, About}

};

</script>