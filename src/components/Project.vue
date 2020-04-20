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
  background-position: top;
  background-size: cover;
  height: 33vh;
  border: solid var(--light-blue) 5px;
  margin: 1em 2em 1em 2em;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  align-items: center;
}
h2 {
  color: var(--white);
  opacity: 1;
}
p {
  margin: 1em 2em;
  padding: 0.5em;
  color: var(--white);
}
p,
.link-container {
  backdrop-filter: blur(5px) brightness(50%);
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
@media only screen and (min-width: 768px) {
  .project {
    flex-direction: row;
    justify-content: left;
    align-items: flex-end;
    width: 80vw;
    height: 40vh;
  }
  p {
    width: 35%;
    padding: 1em;
    margin: 0;
    height: 18vh;
  }
  .link-container {
    flex-direction: column;
  }
}
</style>
