<template>
  <div id="about">
    <h2>
      I've learned a lot over the past few months!
    </h2>
    <p>
      I've just graduated from a coding bootcamp, General Assembly, in
      Washington, DC. This portfolio showcases a few of my projects.
    </p>
    <div class="link-container">
      <a href="#skills">Skills</a>
      <a href="Sara_Laffin_Resume.pdf" download>
        Resume
      </a>
      <a href="#background">Background</a>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
#about {
  background-color: var(--white);
  display: flex;
  flex-direction: column;
  align-items: center;
}
h2 {
  color: var(--dark-blue);
}
p {
  text-align: center;
  padding: 1em;
  margin-top: 4vh;
}
p,
.link-container {
  margin-bottom: 10vh;
}
.link-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
a {
  margin: 0.2em;
}
</style>
