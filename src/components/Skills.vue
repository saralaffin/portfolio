<template>
  <article id="skills">
    <h2>
      Skills
    </h2>
    <div class="skills-flex">
      <sub-skills
        icon="icon-html5"
        title="Front-end"
        content="HTML ★ CSS ★ JavaScript ★ React ★ Vue ★ Bootstrap ★ Netlify ★ Responsive Design ★ Storybook"
      />
      <sub-skills
        icon="icon-gears"
        title="Back-end"
        content="Node.js ★ Express ★ MongoDB ★ Mongoose ★
              Python ★ Flask ★ Django ★ Peewee ★ SQL ★ PostgreSQL ★ RESTful API ★ Heroku"
      />
      <sub-skills
        icon="icon-linux"
        title="and more!"
        content="Ubuntu Linux ★ Git ★ GitHub ★ Rapid Prototyping  ★ Visual Studio Code ★ MERN Stack "
      />
    </div>
  </article>
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
/* @media only screen and (min-width: 992px) {
  .skills-flex {
    display: flex;
  }
} */
</style>
