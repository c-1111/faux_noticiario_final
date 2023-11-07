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
        // { src: '/popups/cash-in-motion.gif', blinking: false, top: 0, left: 0 },
        // { src: '/popups/normalboom.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups/smiley1.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups/papa_ia.webp', blinking: false , top: 0, left: 0},
        // { src: '/popups/trollface.jpg', blinking: false, top: 0, left: 0 },
        { src: '/popups/sd_card.gif', blinking: false , top: 0, left: 0},
        // { src: '/popups/euros.svg', blinking: false , top: 0, left: 0},
        { src: '/popups/peces.gif', blinking: false , top: 0, left: 0},
        { src: '/popups/moji_fantasma.gif', blinking: false , top: 0, left: 0},
        { src: '/popups/mariposa.gif', blinking: false , top: 0, left: 0},
        // { src: '/popups/computer.gif', blinking: false , top: 0, left: 0},
        { src: '/popups/vigilancia.gif', blinking: false , top: 0, left: 0},
        // { src: '/popups/matrix.gif', blinking: false , top: 0, left: 0},
        // { src: '/popups/data3.gif ', blinking: false , top: 0, left: 0},
        { src: '/popups/nessie.jpg', blinking: false , top: 0, left: 0},
        { src: '/popups/papers.gif', blinking: false , top: 0, left: 0},
        // { src: '/popups/matrix2.gif', blinking: false , top: 0, left: 0},
        // { src: '/popups/ambar.jpg', blinking: false , top: 0, left: 0},
        { src: '/popups/yersov.png', blinking: false , top: 0, left: 0},
        // { src: '/popups/jack_kilby.jpg', blinking: false , top: 40, left: 0},
        { src: '/popups/bocadillo.gif', blinking: false , top: 0, left: 0},
        { src: '/popups/moai.png', blinking: false , top: 0, left: 0},
        // { src: '/popups/miku.png', blinking: false , top: 0, left: 0},
        // { src: '/popups/creepy.png', blinking: false , top: 0, left: 0},
        // { src: '/popups/doom.png', blinking: false , top: 0, left: 0},
        { src: '/popups/cam.gif', blinking: false , top: 0, left: 0},
        { src: '/popups/repo.jpg', blinking: false , top: 0, left: 0},
        { src: '/popups/nasa1.gif', blinking: false , top: 0, left: 0},
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
    setInterval(this.randomizeBlinking, 100); // Cambia el estado de parpadeo cada segundo
  },
};
</script>


<style scoped lang="scss">
.imagecontainer
  {
    display: grid;
    overflow-wrap: normal;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr 1fr  1fr 1fr  1fr  1fr ;
    grid-template-rows:1fr 1fr 1fr 1fr 1fr 1fr;
    max-width: 100vw;
    max-height: 100vh;
    overflow:visible;
    img{
      max-width: 250px;
      margin: -50px;
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
