<template>
  <div class="wrapper">
    <div class="square"></div>
    <div class="square"></div>
    <div class="square"></div>
    <div class="square"></div>
    <div class="square"></div>
    <div class="square"></div>
    <div class="square"></div>
    <div class="square"></div>
    <div class="square"></div>
  </div>
</template>


<script>
export default {
  name: "NineSquare",
};
</script>


<style scoped>
.wrapper {
  width: 100%;
  outline: solid 1px teal;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 10px;
}

.wrapper > .square {
  width: 30%;
  outline: solid 1px green;
  padding-top: 30%;
}
</style>