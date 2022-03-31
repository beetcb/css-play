<template>
  <div>
    <div class="center-img">
      <img class="center-me" src="../assets/logo.png" alt="vue-logo" />
    </div>
    <div class="center-div">
      <div class="center-me">Center me, no height</div>
    </div>
  </div>
</template>

<script>
export default {
  name: "center",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.center-img,
.center-div {
  height: 300px;
  width: 100%;
  outline: solid 1px teal;
  margin-bottom: 10px;
}
.center-me {
  outline: solid 1px green;
}

/** Center Image */
/* .center-img {
  display: flex;
  justify-content: center;
  align-items: center;
} */
/* .center-img {
  display: grid;
  justify-content: center;
  align-items: center;
} */
/* .center-img {
  position: relative;
}
.center-img > .center-me {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
} */
/* .center-img {
  display: grid;
}
.center-img > .center-me {
  margin: auto;
} */
/* .center-img {
  display: grid;
  align-items: center;
  justify-items: center;
} */
.center-img {
  display: grid;
  place-items: center;
}

/** Center Div */
/* .center-div {
  display: flex;
  align-items: center;
  justify-content: center;
} */
/* .center-div {
  position: relative;
}
.center-div > .center-me {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
} */
/* .center-div {
  display: grid;
}
.center-div > .center-me {
  margin: auto;
} */
.center-div {
  display: grid;
  align-items: center;
  justify-items: center;
}
</style>