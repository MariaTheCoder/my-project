<template>
  <div class="Displayer">
    <h3>{{headline}}</h3>
    <Button @click="getUsers" buttonText="Load users"/>
    <div v-if="-1 > 0">
      <p>Loading Users...</p>
    </div>
    <div v-else>
      <p>No users are currently loaded</p>
    </div>
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
    data() {
    return {
      users: [],
    }
  },
  methods: {
    getUsers() {
      fetch('https://jsonplaceholder.typicode.com/users')
      .then(response => response.json())
      .then(json => {
        for (let i = 0; i < json.length; i++) {
          console.log(json[i].name);
        }
      })
    },
    updateUsers() {
      //
    }
  },
}
</script>

<style scoped>
  h3 {
    font-weight: bolder;
    font-size: 50px;
  }
</style>