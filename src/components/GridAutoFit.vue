Layout the items in a grid so that:

items have minium width of 100px and fill up the space
place as many items in a row as possible
gap between items is 10px

<template>
  <div class="container">
    <div class="item"></div>
    <div class="item"></div>
    <div class="item"></div>
  </div>
</template>

<style scoped>
.container {
  display: grid;
  gap: 10px;
  grid-template-columns: repeat(auto-fit, minmax(100px, 1fr));
}

.item {
  height: 50px;
  background-color: #7aa4f0;
}
</style>