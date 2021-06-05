<template>
  <div>
    <div class="container">
      <h1 class="title">CONTACTO</h1>
    </div>

    <div class="container9">
      <div class="social">
        <img class="red" src="../static/img/insta.png" />
        <h4>celiaroncero</h4>
      </div>
      <div class="social">
        <img class="red2" src="../static/img/behance.png" />
        <h4>celiaroncero</h4>
      </div>
      <div class="social">
        <img class="red3" src="../static/img/gmail.png" />
        <h4>celiaroncerogmail.com</h4>
      </div>
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
.container9 {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
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
.red{
  width: 150px;
  height: 150px;
  margin-left: 1em;
  margin-right: 1em;
  margin-bottom: 1em;
}
.red2{
  width: 260px;
  height: 150px;
  margin-left: 1em;
  margin-right: 1em;
  margin-bottom: 1em;
}
.red3{
  width: 235px;
  height: 150px;
  margin-left: 1em;
  margin-right: 1em;
  margin-bottom: 1em;
}
</style>
