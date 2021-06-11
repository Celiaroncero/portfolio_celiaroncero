<template>
  <div>
    <div class="container">
      <h1 class="title">SOBRE MÍ</h1>
    </div>

    <div class="container8">
      <img class="celiaimg" src="/img/celia.png" />
 
      <div class="descripcioncelia">
        <div class="nombre">
          <h2>Celia Roncero</h2>

        </div>
         <br />
        Alumna de la Escuela Superior de Diseño de Madrid, actualmente cursando
        tercero en la especialidad de diseño gráfico.
        <br />
        <br />
        Me considero una persona trabajadora, organizada y sociable.
        Acostumbrada a trabajar en equipo con capacidad de adaptación y
        aprendizaje.
      </div>
    </div>
  </div>
</template>

<script>
export default {
  mounted() {
    const controller = new this.$scrollmagic.Controller();

    var scene = new this.$scrollmagic.Scene({ triggerElement: ".container8" })
      // trigger a TweenMax.to tween
      .setTween("#animate1", 0.5, {
        backgroundColor: "white",
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
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.container8 {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  
}
.descripcioncelia {
  width: 690px;
  padding: 3em;
  font-size: 1.3em;
  font-weight: lighter;
  color: rgb(0, 0, 0);
  text-align:left;
 h2{
   color: rgb(255, 153, 0);
 }
  
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

.celiaimg {
  height: 300px;
  width: 300px;
  border-radius: 50%;
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
  color: #000000;
  letter-spacing: 1px;

}

.container8 {
  margin: 0 auto;
  min-height: 70vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  
}
.celiaimg {
  height: 120px;
  width: 120px;
  border-radius: 50%;
  object-fit: cover;
  object-position: center;
  margin-bottom: 6em;
  padding: 1em;
  margin-left: 0.2em ;
}
.descripcioncelia {
  width: 300px;
  font-size: 0.7em;
  font-weight: lighter;
  color: rgb(0, 0, 0);
  text-align:left;
 h2{
   color: rgb(255, 153, 0);
 }
  
}

}
</style>
