<template>
  <div id="app">
    <NavBar />
    <Header />
    <About />
    <Background />
    <Skills />
    <Projects />
    <Contact />
  </div>
</template>

<script>
import NavBar from "./components/NavBar.vue";
import Header from "./components/Header.vue";
import About from "./components/About.vue";
import Background from "./components/Background.vue";
import Skills from "./components/Skills.vue";
import Projects from "./components/Projects.vue";
import Contact from "./components/Contact.vue";

export default {
  name: "App",
  components: {
    Header,
    NavBar,
    About,
    Background,
    Skills,
    Projects,
    Contact,
  },
};
</script>

<style>
:root {
  --black: #04020d;
  --dark-blue: #4679a6;
  --med-blue: #659dbf;
  --light-blue: #8fbdd9;
  --beige: #d9c2a7;
  --white: #fafafa;
}
* {
  box-sizing: border-box;
  margin: 0;
  font-family: "Courier New", Courier, monospace;
}
h1,
h2 {
  font-size: 6vh;
  font-family: "Catamaran", sans-serif;
  color: var(--white);
  margin-top: 15vh;
  text-align: center;
  margin-left: 3vw;
  margin-right: 3vw;
}

a {
  color: var(--white);
  padding: 1.2em;
  background: var(--dark-blue);
  text-decoration: none;
  border-radius: 0.5em;
  text-align: center;
  max-width: 80vw;
}
@media only screen and (min-width: 780px) {
  h1 {
    font-size: 10vh;
    margin-top: 11vh;
  }
}
</style>
