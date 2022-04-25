<script setup>
</script>

<template>
  <div>
    Lorem ipsum dolor sit amet consectetur adipisicing elit. Facere culpa
    suscipit neque inventore in ipsam delectus tenetur ipsum consectetur
    sapiente obcaecati, a architecto sequi aperiam dolor omnis eligendi quas
    amet!
  </div>
</template>

<style scoped>
/* div {
  text-overflow: ellipsis;
  overflow: hidden;
  white-space: nowrap;
} */

div {
  overflow: hidden;
  text-overflow: ellipsis;
  display: -webkit-box;
  /* number of lines to show, n === 2 */
  -webkit-line-clamp: 2;
  line-clamp: 2;
  -webkit-box-orient: vertical;
}
</style>
