Let's create a doughnut chart in CSS.

radius: 50px
thickness: 10px
color: #f44336
The percentage should be able to set by CSS variable --percentage.

For example, to create a doughnut chart with 20%:

<div class="piechart" style="--percentage:20%"></div>

A doughnut chart with 75%:

<div class="piechart" style="--percentage:75%"></div>

<template>
  <div class="piechart" style="--percentage:75%"></div>
</template>


<style scoped>
.piechart {
  width: 100px;
  height: 100px;
  clip-path: circle(50px at center);
  background-image: conic-gradient(#f44336 var(--percentage), transparent 0);
  mask-image: radial-gradient(circle closest-side at center, transparent 80%, #fff 80%);
}
</style>