<template>
  <div class="container">
    <header class="header">header</header>
    <main class="main">main</main>
    <footer class="footer"></footer>
  </div>
</template>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.footer {
  height: 100px;
  background-color: cadetblue;
}

/* Option 1 */
/* .container {
  display: flex;
  flex-direction: column;
  min-height: 100vh;
}

.main {
  flex: 1;
} */

/* Option 2 */
.container {
  display: grid;
  min-height: 100vh;
  grid-template-rows: auto 1fr auto;
}

/* Option 3 */
/* .container {
  min-height: 100vh;
  position: relative;
}

.footer {
  position: absolute;
  width: 100%;
  bottom: 0;
  left: 0;
}

.main {
  margin-bottom: 100px;
  background-color: red;
} */
</style>