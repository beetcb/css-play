<template>
  <div id="contianer">
    <header></header>
    <main id="main"></main>
    <footer id="footer"></footer>
  </div>
</template>

<script>
export default {
  name: "StickyFooter",
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
#contianer {
  min-height: 100vh;
}
#footer {
  height: 100px;
  background: red;
}

/* Option 1 */
/* #contianer {
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}
#main {
  flex: 1 0 auto;
}
#footer {
  flex-shrink: 0;
} */

/* Option 2 */
/* #footer {
  position: sticky;
  top: 100vh;
} */

/* Option 3 */
#contianer {
  position: relative;
}
#footer {
  position: absolute;
  top: 0;
}
</style>