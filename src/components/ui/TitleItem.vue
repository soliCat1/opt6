<template>
  <h1><slot></slot></h1>
</template>

<script>
export default {
  name: 'title-item'
}
</script>

<style scoped>
h1 {
  font-size: 30px;
  margin: 0 0 25px 0;
}
</style>