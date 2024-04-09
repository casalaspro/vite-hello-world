<script>

  import appTitle from './components/appTitle.vue';
  import appHero from './components/appHero.vue';

  export default {
    data(){
      return{
        
      }
    },
    mounted(){
      console.log("Hi! I'm App.vue")
    },
    methods: {

    },
    components : {
      appTitle,
      appHero
    }
  }

</script>

<template>
  <section>
    <appTitle/>
    <appHero/>
  </section>
</template>

<style scoped></style>
