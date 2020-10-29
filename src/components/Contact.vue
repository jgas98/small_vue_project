<template>

  <div class = "header">
    
    <h1 class = "header__title"> Contacta Con Nosotros </h1>

    <br>
    
    <form @submit.prevent = "showUser()"> 
      
      <div class = "form-group">
        
        <label for = "InputUsername"> Nombre </label>
        
        <input type = "text" class = "form-control"  name = "nombre"  v-model = "register.nombre" required>
    
      </div>

      <div class = "form-group">
        
        <label for = "InputUsername"> Apellidos </label>
        
        <input type = "text" class = "form-control" name = "apellidos"  v-model = "register.apellido" required>
    
      </div> 
    
      <div class = "form-group">
        
        <label for = "InputEmail1"> Correo Electronico </label>
        
        <input type = "email" class = "form-control" name = "email" v-model = "register.email" required>
      
      </div>

      <div class = "form-group">
      
        <label> Mensaje </label>
        
        <input type = "text" class = "form-control" name = "mensaje"  v-model = "register.mensaje">
        
      </div>

      <button type = "submit" name = "register" class = "submit-button"> Submit </button>
      
    </form>

  </div>

</template>

<script>

export default {
  
  name: 'register',
  
  data() {
    
    return {
      
      register: {
        
        nombre : " ", 
        
        apellidos : " ", 
        
        email : " ", 
        
        mensaje : " "
        
      }
         
    }
     
  }, methods: {showUser () {console.log(this.register)}}

}

</script>

<style lang = "scss" scoped>

.header {
  
  width: 30%; margin: 40px auto 0px;
  
  text-align: center; padding: 20px; height: auto;
}

.header__title {color: black;}

.form-group {margin: 10px 0px  10px 0px; margin-top: 24px;}

.form-group label {display: block; text-align: left; margin: 3px;}

.form-group input {
  
  height: 30px; width: 93%; padding: 5px 10px;
  
  font-size: 15px; border: 1px solid #D5DBDB; margin: 4px 0;
}

.submit-button {
  
  border: none; padding: 12px 24px;
  
  background-color: aquamarine; color: black;
  
  font-weight: 600; font-size: 14px; margin-top: 24px;
}

</style>