<template>
  <img alt="Vue logo" src="./assets/logo.png">
  <ContentDisplayer headline="HEADLINE"/>
</template>

<script>
import ContentDisplayer from './components/ContentDisplayer.vue';

export default {
  name: 'App',
  components: {
    ContentDisplayer
  }
}
</script>

<style>
#app ,
    ContentDisplayer{
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}
</style>
