Create a heading of fluid font size.

if viewport width is smaller than 200px, use 16px
if viewport width is bigger than 400px, use 32px
otherwise font-size is linearly scaled. For example 
if viewport is 300px = (200px + 400px) / 2, then font-size is 24px = (16px + 32px) / 2

<template>
  <h1 class="title">BFE.dev</h1>
</template>

<style scoped>
.title {
  text-align: center;
  /* 
  200px * 0.08 = 16px; -> min
  400px * 0.08 = 32px; -> between the min and max, 8vw 
  300px * 0.08 = 24px; -> max 
  */
  font-size: clamp(16px, 8vw, 32px);
}


/* Option 2 */
.title {
  text-align: center;
  font-size: 8vw;
}

@media screen and (max-width: 200px) {
  .title {
    font-size: 16px;
  }
}

@media screen and (min-width: 400px) {
  .title {
    font-size: 32px;
  }
}
</style>