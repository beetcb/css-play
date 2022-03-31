
<template>
  <div class="container">
    <div id="mar-a">a</div>
    <div id="mar-b"></div>
  </div>
</template>

<script>
export default {
  name: "MarginColl",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#mar-a {
  margin-bottom: 100px;
  outline: solid 1px yellowgreen;
}
#mar-b {
  margin-top: 100px;
  margin-bottom: 100px;
  outline: solid 1px yellowgreen;
}
</style>