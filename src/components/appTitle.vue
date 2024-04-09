<script>

  export default {
    data(){
      return{
        title : "La mia prima app con",
      }
    },
    mounted(){
      console.log("Hi i'm appTitle");
    }
  }



</script>

<template>
  <section>
    <h1>{{ title }}</h1>
  </section>
</template>

<style scoped>


  h1{
    text-align: center;
    color: white;
    font-size: xx-large;
    letter-spacing: 2px;
    margin: 20px;
  }

</style>