<template>
  <label class="my-checkbox">
    <input type="checkbox" />
    <span>a checkbox</span>
  </label>
</template>

<style scoped>
/* More advanced guide https://moderncss.dev/pure-css-custom-checkbox-style/ */
.my-checkbox {
  display: flex;
  /* justify-content: center; */
}

.my-checkbox > input[type="checkbox"] {
  appearance: none;
  align-self: center;
  width: 10px;
  height: 10px;
  border: none;
  border-radius: 50%;
  background-color: gray;
}

.my-checkbox > input[type="checkbox"]:checked {
  background-color: green;
}
</style>