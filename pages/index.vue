<template>
  <div>
    
    <div class="container">
      <h1 class="title">CELIA RONCERO</h1>
    </div>

    <div class="container2">
      <span id="animate1" style="transform: rotate(360deg) width: 150px; height:100px;border-radius:50%;">
      <img class="cevlogo" src ="/img/cev.png">  
      </span>
    </div>
    <div class="container2-1">
      <div class="definicion">
        <h2>Cultura en Vena</h2>
         <br>
        Cultura en Vena es una fundación que nace en diciembre de 2019 y se
        encarga de mejorar la vida de las personas vinculando la cultura con la
        salud y el bienestar. 
        <br>
        <br>Acercan el arte y la música a los entornos sanitarios y a regiones en riesgo de despoblación. También investigan
        los efectos de las prácticas artísticas en la salud y el bienestar con
        el objetivo de aumentar las evidencias sobre la contribución de las
        artes tanto a la promoción y prevención de la salud y el bienestar, como
        a la gestión y tratamiento de estas.
      </div>
    </div>
    <div class="container2-2">
      <div class="imgcev">
      <img src="/img/444.png">
      </div>
    </div>
    <div class="container3">
      <span id="animate2"><img class="filminlogo" src ="/img/filmin.png"></span>
    </div>
    
    <div class="containerpromo">
     
     <video class="videopromo"
          src="/img/promo.mp4"
          controls
          loop
          width="100%"
        ></video>
     
    </div>
    <div class="container4">
      
      <div class="definicionfilmin">
        <h3>FILMIN</h3>
        <br>
        Filmin es una plataforma de contenido en línea española creada en 2007
        con el objetivo de ofrecer contenido para cinéfilos y fomentar un
        sentido de red social.  
         <br>
         <br>Consideramos que algunos de
        los grandes problemas de filmin son tanto la falta de adaptación del
        diseño a los diferentes formatos existentes, como la mala organización
        del contenido a lo largo de toda la interfaz que trae consigo una pésima
        experiencia de usuario. Así como la evidente desvinculación que hay
        entre el tono que pretenden dar y el que realmente generan en la
        gráfica.
      </div>
      
    </div>
    <div class="container5">
     
      <div class="imgfilmin">
     <img src="/img/filmindos.png">
     
    
     </div>
    </div>
    <div class="container6">
      
      <img class="discologo" src="/img/sebastian.png">
     
    </div>
    <div class="container7">
      
      <div class="textdisco">
       <h2> Rediseño Yo q se </h2>
       <br>
       Rediseño del single "Yo q se" del Artista sebastian cortes, en el cual mediante ilustración adapto 
       la gráfica del disco a las sensaciones que realmente transmite la canción y la personalidad del artista.
       

      </div>
    </div>
     <div class="containerdisco">
      
      <img class="discoimg" src="/img/disco.png">
     
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    const controller = new this.$scrollmagic.Controller();

    var scene = new this.$scrollmagic.Scene({ triggerElement: ".container2" })
      // trigger a TweenMax.to tween
      .setTween("#animate1", 0.5, {
        backgroundColor: "none",
        scale: 2.5,
        rotate: 360,
      })
      .addTo(controller);

 
    var scene2 = new this.$scrollmagic.Scene({
      triggerElement: ".container3",
      duration: 300,
    })
      // trigger a TweenMax.to tween
      .setPin("#animate2")
      // add indicators (requires plugin)
      //.addIndicators({name: "1 (duration: 300)"})
      //.setTween("#animate2", 0.5, {backgroundColor: "white"})
      .addTo(controller);
  },
};
</script>

<style lang="scss">
.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 90px !important;
  color: #000000 ;
  letter-spacing: 1px;
}
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.container2 {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: linear-gradient(#39AE6F 0%, #75C9F2 100%,);
}
.container2-1 {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: white;
 
  .definicion {
    width: 800px;
    font-size: 30px  !important;
    color: rgb(77, 77, 77);
    font-weight: lighter;
    h2{
      color:#F5BD2D ;
    }
  }
}
.container2-2 {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: white;
}

.container3 {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: linear-gradient(#07E8BF 0%, #0F1E27 100%) !important;
  font-size: 80px;
}
.container4 {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: white;

  .definicionfilmin {
    width: 800px;
    font-size: 25px;
    color: rgb(77, 77, 77);
    font-weight: lighter;
    h3{
       font-size: 40px;
       color: #07E8BF;
    }
    
    
  }
  .titulofilmin{
      color:#0F1E27;
      font-size: 30px;
    }
}

.container5 {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: white !important;
  
}
.containerpromo {
    margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  font-size: 80px;
  color:white;
  background-color:  #0F1E27;
  .videopromo{
   width: 100%;
   width: 100%
  }
}
.container6 {
    margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  font-size: 80px;
  color:white;
  background-color: rgb(54, 162, 201);
}
.container7 {
  display: grid;
  justify-content: center;
    margin: 0 auto;
  min-height: 100vh;
  text-align: center;
  font-size: 1.3em;
  color:rgb(85, 85, 85);
  background-color: rgb(255, 255, 255);
  
  h2{
    color:rgb(54, 162, 201);
    
  }
}
.containerdisco {
    margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  font-size: 80px;
  color:white;
  background-color: rgb(255, 255, 255);
 
}
 .textdisco{
  
  font-weight: lighter;
  font-size: 28px;
  width: 600px !important;
 margin-top: 2em;
  
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

.imgcev{
  width: 80rem;
  
  
  
  img{
    height: 100%;
    width: 100%;
    object-fit: cover;
    object-position: center;
  }
}
.imgfilmin{
  width: 60rem;
  margin-top: -20rem;
  
  img{
    height: 100%;
    width: 100%;
    object-fit: cover;
    object-position: center;
  }
}
.cevlogo{
   height: 100px;
    width: 100px;
    object-fit: cover;
    object-position: center;
    
}
.filminlogo{
   height: 100%;
    width: 100%;
    object-fit: cover;
    object-position: center;

}
.discologo{
 height: 520px;
    width: 520px;
    object-fit: cover;
    object-position: center;
}
.discoimg{
 height: 550px;
    width: 800px;
    object-fit: cover;
    object-position: center;
}


@media screen and (max-width: 600px) {
.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 60px !important;
  color: #000000 ;
  letter-spacing: 1px;
}
.container2 {
  margin: 0 auto;
  min-height: 80vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: linear-gradient(#39AE6F 0%, #75C9F2 100%,);
}
.cevlogo{
   height: 65px;
    width: 65px;
    object-fit: cover;
    object-position: center;
    
}
.container2-1 {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: white;
 
  .definicion {
    width: 800px;
    font-size: 22px  !important;
    padding: 1.5em;
    color: rgb(77, 77, 77);
    font-weight: lighter;
    h2{
      color:#F5BD2D; 
      padding: 0.5em;
      margin-top: em;
    }
  }
}
.container2-2 {
  margin: 0 auto;
  min-height: 30vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: white;
  margin-bottom: 5em;
}
.container3 {
  margin: 0 auto;
  min-height: 80vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: linear-gradient(#07E8BF 0%, #0F1E27 100%) !important;
  font-size: 80px;
}
.filminlogo{
   height: 60%;
    width: 60%;
    object-fit: cover;
    object-position: center;
    padding: 0.2em;

}
.containerpromo {
    margin: 0 auto;
  min-height: 50vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  font-size: 80px;
  color:white;
  background-color:  #0F1E27;
  .videopromo{
   width: 100%;
   width: 100%
  }
}
.container4 {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background: white;

  .definicionfilmin {
    width: 800px;
    font-size: 21px;
    color: rgb(77, 77, 77);
    font-weight: lighter;
    padding: 1.5em;
    h3{
       font-size: 40px;
       color: #07E8BF;
    }
    
    
  }
  .titulofilmin{
      color:#0F1E27;
      font-size: 30px;
    }
}
.container5 {
  margin: 0 auto;
  min-height: 50vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  background-color: white !important;
  
}
.imgfilmin{
  width: 60rem;

  img{
    margin-top: 4em;
    height: 100%;
    width: 100%;
    object-fit: cover;
    object-position: center;
  }
}

.container6 {
    margin: 0 auto;
  min-height: 80vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  font-size: 80px;
  color:white;
  background-color: rgb(54, 162, 201);
}
.discologo{
 height: 85%;
    width: 85%;
    object-fit: cover;
    object-position: center;
}
}


.container7 {
   margin-top: 4em ;
 
  min-height: 60vh;
  text-align: center;
  font-size: 1em;
  color:rgb(85, 85, 85);
  background-color: rgb(255, 255, 255);
  
  h2{
    color:rgb(54, 162, 201);
    
    
  }
}
.containerdisco {
    margin: 0 auto;
  min-height: 10vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  font-size: 80px;
  color:white;
  background-color: rgb(255, 255, 255);
  margin-bottom: 2em;
 
}
.discoimg{
 height: 80%;
    width: 80%;
    object-fit: cover;
    object-position: center;
}
@media screen and (max-width: 600px) {
  .textdisco{
  font-weight: lighter;
  font-size: 22px;
  width: 350px !important;
  padding: 1em;
  
  }
}

</style>
