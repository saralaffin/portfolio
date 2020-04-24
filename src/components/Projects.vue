<template>
  <article id="projects">
    <h2>
      Projects
    </h2>
    <div class="projects-grid">
      <project
        id="pawsitivity"
        description="Developed a mock Instagram MVP utilizing a MERN stack in 4.5
                    days with a team of 4 people"
        githubURL="https://github.com/saralaffin/best-in-show"
        deployedURL="https://pawsitivity.netlify.com/"
      />
      <project
        id="cotripper"
        description="Contributed to an open source, full stack travel application for single mothers built using Django and React"
        githubURL="https://github.com/CotripperPlatform/CoTrip"
        deployedURL="https://cotripper.netlify.app/"
      />
      <project
        id="hanoi"
        description="Built front end game using HTML, CSS, and vanilla JavaScript"
        githubURL="https://github.com/saralaffin/front-end-game-tower-of-hanoi"
        deployedURL="https://saralaffin.github.io/front-end-game-tower-of-hanoi/"
      />
      <project
        id="clean"
        description="Utilized HTML and custom CSS to build a responsive website
                    showcasing service for a cleaning company"
        githubURL="https://github.com/saralaffin/responsive-website"
        deployedURL="https://saralaffin.github.io/responsive-website/"
      />
    </div>
  </article>
</template>

<script>
import Project from "./Project.vue";
export default {
  name: "Projects",
  props: {
    msg: String,
  },
  components: {
    Project,
  },
};
</script>

<style scoped>
#projects,
.projects-grid {
  background-color: var(--dark-blue);
  display: flex;
  flex-direction: column;
  align-items: center;
}
h2 {
  color: var(--white);
  opacity: 1;
}
#pawsitivity {
  background-image: url("../assets/pawsitivity.png");
}
#cotripper {
  background-image: url("../assets/cotripper.png");
}
#hanoi {
  background-image: url("../assets/tower-of-hanoi.png");
}
#clean {
  background-image: url("../assets/responsive-website.png");
}
@media only screen and (min-width: 992px) {
  .projects-grid {
    width: 80vw;
    height: 80vw;
    display: grid;
    grid-template-columns: repeat(5, 1fr);
    grid-template-rows: repeat(6, 1fr);
    grid-gap: 1em;
    margin: 1em;
  }
  #pawsitivity {
    grid-column: 1 / span 3;
    grid-row: 1 / span 3;
  }
  #hanoi {
    grid-column: 4 / span 2;
    grid-row: 2 / span 2;
  }
  #clean {
    grid-column: 1 / span 2;
    grid-row: 4 / span 2;
  }
  #cotripper {
    grid-column: 3 / span 3;
    grid-row: 4 / span 3;
  }
}
</style>
