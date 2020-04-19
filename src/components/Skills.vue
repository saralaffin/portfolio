<template>
  <div id="skills">
    <h2>
      Skills
    </h2>
    <sub-skills
      icon="icon-pencil"
      title="Languages"
      content="HTML, CSS, JavaScript, Python, SQL"
    />
    <sub-skills
      icon="icon-edit"
      title="Frameworks/libraries"
      content="Bootstrap, Django, Express, Flask, Git, MERN Stack, Mongoose,
              Node.js, Peewee, React, Vue"
    />
    <sub-skills
      icon="icon-envelope-alt"
      title="and more!"
      content="APIs, Github, Heroku, MongoDB, Netlify, PostgreSQL, Responsive
              Design, RESTful API, Storybook, Ubuntu Linux, Visual Studio Code"
    />
  </div>
</template>

<script>
import SubSkills from "./SubSkills.vue";

export default {
  name: "Skills",
  components: {
    SubSkills,
  },
};
</script>

<style scoped>
#skills {
  background-color: var(--white);
  display: flex;
  flex-direction: column;
  align-items: center;
}
h2 {
  color: var(--dark-blue);
}
</style>
