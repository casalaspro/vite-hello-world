<script>

export default {
  data(){
    return{
      imageName : "landscape.jpg"
    }
  },
  methods: {
    getImagePath(img){
      return new URL(`../assets/${img}`, import.meta.url).href
    }

  },

  mounted(){
    console.log("appHero!")
    console.log(this.getImagePath(this.imageName))
  }
}

</script>

<template>
  <section class="hero" :style="{ backgroundImage: 'url(' + getImagePath(imageName) + ')' }">
    <!-- <img :src="getImagePath(imageName)"> -->
    <h2>VITE!</h2>

  </section>

</template>

<style scoped>
 .hero{
  height: 400px;
  background-position: center;
  background-size: cover;
  display: flex;
  justify-content: center;
  align-items: center;
 }

 h2{
  font-size: 200px;
  color: rgba(255, 255, 255, 0.851);
 }



</style>