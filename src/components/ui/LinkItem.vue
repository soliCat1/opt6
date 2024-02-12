<template>
  <li :class="{active: $props.link.isActive}">{{ $props.link.name }}</li>
</template>

<script>
export default {
  name: 'link-item',
  props: {
    link: {
      type: Object
    }
  }
}
</script>

<style scoped lang="scss">
li {
  font-size: 16px;
  font-weight: 600;
  color: #1253a2;
  cursor: pointer;

  &:hover {
    color: #000000;
  }
}

.active {
  color: #000000;
}
</style>