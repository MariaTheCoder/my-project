<template>
  <div class="Displayer">
    <ul>Hello {{headline}}</ul>
  </div>
</template>

<script>
export default {
  name: 'ConcentDisplayer',
  props: {
    headline: String,
  }
}
</script>

<style scoped>
  ul {
    font-weight: bolder;
    font-size: 100px;
  }
</style>