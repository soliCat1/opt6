<template>
  <div class="wrapper">
    <side-bar />
    <section class="container">
      <title-item>Проведение ТО и мелкий ремонт</title-item>
      <link-list></link-list>
      <top-section></top-section>
      <table-section></table-section>
    </section>
  </div>
</template>

<script>
export default {

}
</script>

<style>
*,
*::after,
*::before {
  box-sizing: border-box;
}

@font-face {
  font-family: "MyriadPro";
  font-style: normal;
  font-weight: 400;
  src: url("../src/assets/fonts/MYRIADPRO-REGULAR.OTF")format("opentype");
  font-display: swap;
}

@font-face {
  font-family: "MyriadPro";
  font-style: normal;
  font-weight: 600;
  src: url("../src/assets/fonts/MYRIADPRO-SEMIBOLD.OTF")format("opentype");
  font-display: swap;
}

body {
  margin: 0;
  padding: 0;
  font-family: "MyriadPro", sans-serif;
  font-weight: 400;
  font-size: 16px;
  color: #000000;
}

.wrapper {
  display: flex;
}

.container {
  padding: 25px;
  flex-grow: 1;
  background-color: #fbfcfd;
}
</style>
