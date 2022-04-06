1. when viewport width is not enough, set left column to 40px wide and middle column to stretching.
2. middle column has maximum width of 240px
3. when there is enough space, show right column which has width of 120px
4. if there is more space, set left column to 80px
5. when right column is visible, set minimum 10px space horizontally to the viewport border

<template>
  <div class="container test">
    <div class="left">left</div>
    <div class="middle">middle</div>
    <div class="right">right</div>
  </div>
</template>


<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 150px;
}

.left,
.middle,
.right {
  display: grid;
  place-items: center;
  height: 100%;
}

.left {
  width: 40px;
  background-color: #eee;
}
.middle {
  max-width: 240px;
  flex: 1;
  background-color: #ddd;
}
.right {
  display: none;
  background-color: #eee;
}

@media screen and (min-width: 420px) {
  .container {
    margin: 0 min(10px);
  }
  .right {
    display: grid;
    width: 120px;
  }
}

@media screen and (min-width: 460px) {
  .left {
    width: 80px;
  }
}
</style>