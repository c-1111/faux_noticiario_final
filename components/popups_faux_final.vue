<template>
 <div class="popups">   
    <div class="imagecontainer">
      <img v-for="(image, index) in images" :key="index" :src="image.src" />
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      images: [
        { src: '/faux_3d.gif'},
        { src: '/tagline.png' },

      ],
    };
  },
};
</script>


<style scoped lang="scss">
.imagecontainer
  {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    overflow-wrap: normal;
    max-width: 100vw;
    max-height: 100vh;
    img{
      max-width: 400px;
      margin-left: 1%;
      margin-top: 1%;
      background: #fff;
      padding: 2rem;
      border: solid 1px #000;
      
    } @media (max-width: 600px) {
      max-width: 200px;
      margin-left: 30%;
      margin-top: 5%;
      gap: 4rem;
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
