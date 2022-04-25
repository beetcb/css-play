<template>
  <ol>
    <li>BFE.dev</li>
    <li>
      JavaScript
      <ol>
        <li>TypeScript</li>
        <li>Quiz</li>
        <li>
          Framework
          <ol>
            <li>React</li>
            <li>Vue.js</li>
          </ol>
        </li>
      </ol>
    </li>
    <li>CSS</li>
    <li>System Design</li>
  </ol>
</template>

<style scoped>
ol {
  list-style-type: none;
  counter-reset: ol-list;
  margin-left: -13px;
}

li::before {
  color: #f44336;
  counter-increment: ol-list;
  /* Concat ol-list counters */
  content: counters(ol-list, ".") " ";
}
</style>