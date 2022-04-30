Implement Holy Grail Layout which includes header, left sidebar, body, right sidebar and footer.

it should be sticky footer
left sidebar and right sidebar should be fixed width of 100px.
styles of color .etc are already set for you, only layout related CSS code is needed.

<template>
  <div class="container">
    <header class="header">header</header>
    <div class="left-sidebar">left sidebar</div>
    <div class="body">body</div>
    <div class="right-sidebar">right sidebar</div>
    <footer class="footer">footer</footer>
  </div>
</template>


<style scoped>
/* Option 1 */
.container {
  display: grid;
  min-height: 100vh;
  grid-template-columns: 100px 1fr 100px;
  grid-template-rows: auto 1fr auto;
}

.header,
.footer {
  grid-column: 1/4;
}
</style>