<template>
  <div class="button">
    <button>{{buttonText}}</button>
  </div>
</template>

<script>
export default {
  name: 'Button',
  props: {
    buttonText: String,
  }
}
</script>

<style scoped>
</style>