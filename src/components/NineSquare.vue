<template>
  <div class="wrapper">
    <div class="square">1</div>
    <div class="square">2</div>
    <div class="square">3</div>
    <div class="square">4</div>
    <div class="square">5</div>
    <div class="square">6</div>
    <div class="square">7</div>
    <div class="square">8</div>
    <div class="square">9</div>
  </div>
</template>


<script>
export default {
  name: "NineSquare",
};
</script>


<style scoped>
/* Hack, hard to maintain
.wrapper {
  width: 100%;
  outline: solid 1px teal;
  margin: 0 auto;
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  gap: 10px;
}

.wrapper>.square {
  width: 30%;
  outline: solid 1px green;
  padding-top: calc(30% - 18.5px);
} */

.wrapper {
  display: grid;
  grid-template-rows: repeat(3, 1fr);
  grid-auto-flow: column;
  gap: 10px;
}

.square {
  aspect-ratio: 1;
  display: flex;
  align-items: center;
  background-color: #7aa4f0;
  justify-content: center;
}
</style>