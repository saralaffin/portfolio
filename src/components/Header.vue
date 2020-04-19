<template>
  <div class="header">
    <h1>SARA LAFFIN</h1>
    <a href="#about">Meet your company's next software engineer!</a>
  </div>
</template>

<script>
export default {
  name: "Header",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
.header {
  background-image: url("../assets/mesaverde.jpg");
  height: 100vh;
  width: 100vw;
  background-position: center;
  background-size: cover;
  display: flex;
  flex-direction: column;
  align-items: center;
}
h1 {
  opacity: 0.85;
}
a {
  margin-top: 40vh;
  opacity: 0.85;
}
</style>
