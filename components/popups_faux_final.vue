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
        { src: '/faux_3d_lag.gif'},

      ],
    };
  },
};
</script>


<style scoped lang="scss">
.imagecontainer
  {
    display: flex;
    justify-content: center;
    align-items: center;
    overflow-wrap: normal;
    max-width: 100vw;
    max-height: 100vh;
    img{
      width: 1400px;
      margin-left: 10%;
      margin-top: 10%;

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
