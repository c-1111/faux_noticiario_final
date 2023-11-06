<template>
 <div class="popups">   
    <div class="imagecontainer">
      <img v-for="(image, index) in images" :key="index" :src="image.src" :class="{ 'blinkingimage': image.blinking }" />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      images: [
        { src: '/popups3/bengalas.jpg', blinking: false, top: 0, left: 0 },
        { src: '/popups3/camcorder.png', blinking: false, top: 0, left: 0 },
        { src: '/popups3/camcorder2.jpg', blinking: false, top: 0, left: 0 },
        { src: '/popups3/cap.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups3/coche.jpg', blinking: false, top: 0, left: 0 },
        { src: '/popups3/danger.png', blinking: false, top: 0, left: 0 },
        { src: '/popups3/dog.png', blinking: false, top: 0, left: 0 },
        { src: '/popups3/ecp.jpg', blinking: false, top: 0, left: 0 },
        { src: '/popups3/gameoflife.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups3/heli.gif', blinking: false, top: 0, left: 0 },
        // { src: '/popups3/kirby.gif', blinking: false, top: 0, left: 0 },
        // { src: '/popups3/laser.png', blinking: false, top: 0, left: 0 },
        { src: '/popups3/manfire.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups3/minidisc.jpg', blinking: false, top: 0, left: 0 },
        { src: '/popups3/nasalogo.png', blinking: false, top: 0, left: 0 },
        { src: '/popups3/piss_christ.jpg', blinking: false, top: 0, left: 0 },
        { src: '/popups3/play.png', blinking: false, top: 0, left: 0 },
        // { src: '/popups3/print.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups3/sea.jpg', blinking: false, top: 0, left: 0 },
        { src: '/popups3/sky_billboard.jpg', blinking: false, top: 0, left: 0 },
        { src: '/popups3/srta.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups3/whitecomp.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups3/stairs.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups3/subway guide.jpg', blinking: false, top: 0, left: 0 },





        // { src: '', blinking: false , top: 0, left: 0},
      ],
    };
  },
  methods: {
    randomizeBlinking() {
      this.images.forEach((image) => {
        image.blinking = Math.random() < 0.5; // Controla si la imagen parpadea o no
      });
    },
  },
  mounted() {
    this.randomizeBlinking();
    setInterval(this.randomizeBlinking, 300); // Cambia el estado de parpadeo cada segundo
  },
};
</script>


<style scoped lang="scss">
.imagecontainer
  {
    display: grid;
    overflow-wrap: normal;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr  1fr 1fr  ;
    grid-template-rows:1fr 1fr 1fr 1fr ;
    max-width: 100vw;
    max-height: 100vh;
    overflow:visible;
    img{
      max-width: 200px;
      margin: 1rem;
    }
  }
  .blinkingimage {
    opacity: 0;
    animation: blink infinite;
  }

  @keyframes blink {
    0% {
      opacity: 0;
    }
    50% {
      opacity: 1;
    }
    100% {
      opacity: 0;
    }
  }
</style>
