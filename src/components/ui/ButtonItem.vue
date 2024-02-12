<template>
  <button type="button">
    <slot></slot>
    </button>
</template>

<script>
export default {
  name: 'button-item'
}
</script>

<style>
button {
  padding: 10px 15px 10px 28px;
  border-radius: 5px;
  background-color: #2f8cff;
  border: none;
  background-image: url("../../assets/img/plus.svg");
  background-repeat: no-repeat;
  background-position: 10px center;
  font-size: 14px;
  color: #ffffff;
  font-family: "MyriadPro", sans-serif;
  cursor: pointer;
}
</style>