<template>
  <div>
    

    <div class="container9">
     <div class="galeria">
          <img class="imggaleria" src ="/galeria/1.png">
          <img class="imggaleria" src ="/galeria/2.png">  
          <img class="imggaleria" src ="/galeria/3.png">  
          <img class="imggaleria" src ="/galeria/4.png">  
          <img class="imggaleria" src ="/galeria/5.png">     
     </div>
    </div>
     <div class="container9">
   
       <div class="galeria">
          <img class="imggaleria" src ="/galeria/6.png">
          <img class="imggaleria" src ="/galeria/7.png">  
          
     </div>
    
    </div>
     <div class="container9">

     <div class="galeria">
          <img class="imggaleria" src ="/galeria/8.png">
            <img class="imggaleria" src ="/galeria/9.png">
          <img class="imggaleria" src ="/galeria/10.png">
          
     </div>
    
    </div>
  </div>
</template>

<script>


</script>

<style lang="scss">

.container9 {
  margin: 0 auto;
  min-height: 10vh !important;
  
  justify-content: center;
  align-items: center;
  text-align: center;
}
.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 90px;
  color: #000000;
  letter-spacing: 1px;
}
.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #000000;
  word-spacing: 5px;
  padding-bottom: 15px;
}
.links {
  padding-top: 15px;
}
.imggaleria{
     width: 70%;
     height: 70%;
       padding: 0.2em;

    } 
.galeria{
  display: flex; 
}

@media screen and (max-width: 600px) {
.galeria{
  display: grid;


    .imggaleria{

     width: 100%;
     height: 100%;
       padding: 0.2em;

    }  
}
}




</style>
