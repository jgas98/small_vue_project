<template>
  
  <section>
    
    <nav class = "sticky NavGrid-container">
    
      <div class = "NavGrid-item">
    
        <ul class = "navbar">
    
          <li> <router-link to = "/"> Home </router-link> </li>
          
          <li> <router-link to = "/register"> Contacta con Nosotros </router-link>  </li>
        
        </ul>
      
      </div>
    
    </nav>
    
   
    <div style = "padding-top: 10vh;">
      
      <div class = "Box">
        
        <img src = "https://storage-asset.msi.com/event/spb/2019/best-gaming-desktop-pc/images/kv-pd.png" width = "70%" height = "10%" alt = "componenentes_cutre" >

      </div>
      
    </div>
  
  </section>

</template>

<script>

export default {};

</script>

<style lang = "scss" >

.Box {padding-top: 20px; padding-bottom: 20px; display: flex; justify-content: center;}

.navbar {display: flex; list-style: none; width: 100%; justify-content: center; align-self: center;}

.sticky {overflow: hidden; position: fixed; top: 0; width: 100%;}

.navbar li {align-self: center; padding-right: 20px;}

.navbar li a {padding-left: 20px;}

</style>
