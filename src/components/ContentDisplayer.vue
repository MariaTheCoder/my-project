<template>
  <div class="Displayer">
    <h3>{{headline}}</h3>
    <Button @click="getUsers" buttonText="SOME TEXT"/>
  </div>
</template>

<script>
import Button from './Button.vue'

export default {
  name: 'ConcentDisplayer',
  props: {
    headline: String,
  },
  components: {
    Button,
  },
  methods: {
    getUsers() {
      fetch('https://jsonplaceholder.typicode.com/users')
      .then(response => response.json())
      .then(json => console.log(json))
    }
  }
}
</script>

<style scoped>
  h3 {
    font-weight: bolder;
    font-size: 50px;
  }
</style>