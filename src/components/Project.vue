<template>
  <div class="project">
    <p>
      {{ description }}
    </p>
    <div class="link-container">
      <a :href="githubURL" target="_blank"><i class="icon-github"></i></a>
      <a :href="deployedURL" target="_blank">
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
  height: 50vh;
  border: solid var(--light-blue) 5px;
  display: flex;
  flex-direction: column;
  justify-content: center;
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
  margin: 1vw;
  height: 8vw;
  width: 8vw;
  font-size: 5vw;
  padding: 1vw;
  display: flex;
  justify-content: center;
  align-items: center;
}
@media only screen and (min-width: 768px) and(max-width: 992px) {
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
@media only screen and (min-width: 768px) {
  .project {
    width: 100%;
    height: 100%;
  }
}
@media only screen and (min-width: 992px) {
  .project {
    width: 100%;
    height: 100%;
    flex-direction: column-reverse;
    justify-content: flex-start;
    align-items: flex-start;
  }
  p {
    width: 50%;
    min-height: 96px;
    padding: 1em;
    margin: 0;
    display: none;
  }
  .project:hover > p {
    display: block;
  }
  a {
    height: 64px;
    width: 64px;
    font-size: 32px;
    margin: 16px;
  }
}
</style>
