<template>
  <ul>
    <link-item v-for="link in links" :key="link.name" :link="link"></link-item>
  </ul>
</template>

<script>
export default {
  name: 'link-list',
  data: () => ({
    links: [
      {
        name: 'Общее',
        isActive: false
      },
      {
        name: 'Товары',
        isActive: true
      },
      {
        name: 'Доп. расходы',
        isActive: false
      }
    ]
  })
}
</script>

<style scoped>
ul {
  display: flex;
  gap: 20px;
  list-style: none;
  padding: 0;
  margin: 0 0 25px 0;
}
</style>
