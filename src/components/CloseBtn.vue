<template>
  <button class="close test"></button>
</template>

<style scoped>
.test {
  width: 200px;
  height: 200px;
}

.close {
  border: 1px solid #aaa;
  border-radius: 50%;
  position: relative;
}

.close::before,
.close::after {
  content: "";
  position: absolute;
  background-color: #aaa;
  width: 75%;
  height: 2px;
}

.close::before {
  transform: translate(-50%, -50%) rotate(45deg);
}
.close::after {
  transform: translate(-50%, -50%) rotate(-45deg);
}
</style>