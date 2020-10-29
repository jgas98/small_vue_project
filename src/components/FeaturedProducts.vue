<template>
 
  <div>
  
    <p style = "text-align: center; font-size: 40px;"> Productos de Pacotilla </p>
  
    <div class = "container">
  
      <div v-for = "product in products" :key = "product.ProductId">
  
        <div style = "padding-right: 20px;" class = "products">
  
          <img class = "img" :src = "product.image" :alt = "product.title"/>
  
          <div class = "prod_info">
  
            <p class = "title"> {{product.title}} </p>
    
            <p class = "price"> {{product.price}} $ </p>
  
          </div>
  
        </div>
  
      </div>
  
    </div>
  
  </div>

</template>

<script>

export default {
  
  name: "products",
  
  data() {
    
    return {
      
      products: [

         {title: "Google Phone", price: "200", image: "https://static.carrefour.es/hd_350x_/imagenes/products/88016/43863/982/8801643863982/imagenGrande1.jpg"},

         {title: "Samsung S7", price: "2000", image: "https://static.carrefour.es/hd_350x_/imagenes/products/50252/32889/617/5025232889617/imagenGrande1.jpg"},
  
         {title: "HTC 10", price: "1200", image: "https://static.carrefour.es/hd_350x_/crs/cdn_static/catalog/hd/035689_00_1.jpg"},
  
         {title: "iPhone", price: "4200", image: "https://static.carrefour.es/hd_350x_/crs/cdn_static/catalog/hd/322130_00_1.jpg"},
  
         {title: "Samsung A8", price: "8200", image: "https://static.carrefour.es/hd_350x_/imagenes/products/42503/66850/313/4250366850313/imagenGrande1.jpg"},
  
         {title: "Huawei S3", price: "200", image: "https://static.carrefour.es/hd_350x_/imagenes/products/42503/66836/263/4250366836263/imagenGrande1.jpg"},
  
         {title: "HTC 8", "price": "3200", "image": "https://static.carrefour.es/hd_350x_/crs/cdn_static/catalog/hd/865939_00_1.jpg"},
        
         {title: "Google Phone", price: "12200", image: "https://static.carrefour.es/hd_350x_/imagenes/products/84365/42857/499/8436542857499/imagenGrande1.jpg"},

         {title: "Google Phone", price: "12200", image: "https://static.carrefour.es/hd_350x_/imagenes/products/20191/03102/550/2019103102550/imagenGrande1.jpg"}
      
      ]
    
    };
  
  },
  
  methods: {}

};

</script>

<style lang = "scss" >

.img {display: block; margin-left: auto; margin-right: auto; width: 80%;}

.container {display: flex; justify-content: center; align-items: center; flex-wrap: wrap;}

.products {border-radius: 5px; border: solid 1px silver; margin: 20px;}

.prod_info {text-align: center;
  
  .title {font-size: 20px;}

}

</style>