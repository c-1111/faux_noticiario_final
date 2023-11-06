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
        { src: '/popups2/comp_geometric.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups2/books.jpeg', blinking: false, top: 0, left: 0 },
        { src: '/popups2/man.png', blinking: false, top: 0, left: 0 },
        { src: '/popups2/skynet.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups2/iphone.gif', blinking: false, top: 0, left: 0 },
        { src: '/popups2/wifi.jpeg', blinking: false, top: 0, left: 0 },
        { src: '/popups2/flags.png', blinking: false, top: 0, left: 0 },
        { src: '/popups2/music.gif', blinking: false , top: 0, left: 0},
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
    setInterval(this.randomizeBlinking, 4000); // Cambia el estado de parpadeo cada segundo
  },
};
</script>


<style scoped lang="scss">
.imagecontainer
  {
    display: grid;
    overflow-wrap: normal;
    grid-template-columns: 1fr 1fr 1fr 1fr 1fr ;
    grid-template-rows:1fr 1fr 1fr ;
    max-width: 100vw;
    max-height: 100vh;
    overflow:visible;
    img{
      width: 220px;
      height: 400px;
      margin: 3rem;
    }
  }
  .blinkingimage {
    opacity: 0;
    animation: blink 1s infinite;
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
