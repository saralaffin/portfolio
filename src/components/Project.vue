<template>
  <div class="project">
    <p>
      {{ description }}
    </p>
    <div class="link-container">
      <a :href="githubURL"><i class="icon-github"></i></a>
      <a :href="deployedURL">
        <i class="icon-share"></i>
      </a>
    </div>
  </div>
</template>

<script>
export default {
  name: "Project",
  props: {
    description: String,
    githubURL: String,
    deployedURL: String,
  },
};
</script>

<style scoped>
.project {
  background-color: var(--beige);
  background-position: center;
  background-size: cover;
  height: 100vw;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
h2 {
  color: var(--white);
  opacity: 1;
}
.link-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
a {
  margin: 0.2em;
  font-size: 5vh;
  width: 7vh;
  height: 7vh;
  padding: 0.2em;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
