<template>
  <div class="Users">
    <p>{{nameOfUser}}</p>
  </div>
</template>

<script>
export default {
  name: 'Users',
  props: {
    nameOfUser: String,
  },
}
</script>

<style scoped>
p {
  font-weight: bold;
}
</style>