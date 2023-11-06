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
        { src: '/popups_text/ (1).png', blinking: false, top: 0, left: 0 },
        { src: '/popups_text/ (2).png', blinking: false, top: 0, left: 0 },
        { src: '/popups_text/ (3).png', blinking: false, top: 0, left: 0 },
        { src: '/popups_text/ (4).png', blinking: false, top: 0, left: 0 },
        { src: '/popups_text/ (5).png', blinking: false, top: 0, left: 0 },
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
    grid-template-columns: 1fr 1fr  ;
    grid-template-rows:1fr 1fr 1fr ;
    max-width: 100vw;
    max-height: 100vh;
    overflow:visible;
    img{
      max-width: 500px;
      margin: 50px;
      margin-left: 5rem;
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
