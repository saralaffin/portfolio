<template>
  <div id="projects">
    <h2>
      Recent Projects
    </h2>
    <project
      id="pawsitivity"
      description="Developed a mock Instagram MVP utilizing a MERN stack in 4.5
                    days with a team of 4 people"
      githubURL="https://github.com/saralaffin/best-in-show"
      deployedURL="https://pawsitivity.netlify.com/"
    />
    <project
      id="cotripper"
      description="Contributing to an open source, full stack travel application for single mothers built using Django and React"
      githubURL="https://github.com/CotripperPlatform/CoTrip"
      deployedURL="https://cotripper.netlify.app/"
    />
    <project
      id="hanoi"
      description="First front-end project using HTML, CSS, and vanilla JavaScript to build a front-end game"
      githubURL="https://github.com/saralaffin/front-end-game-tower-of-hanoi"
      deployedURL="https://saralaffin.github.io/front-end-game-tower-of-hanoi/"
    />
    <project
      id="clean"
      description="Utilized HTML and custom CSS to build a responsive website
                    showcasing service for a cleaning company. My first General Assembly project!"
      githubURL="https://github.com/saralaffin/responsive-website"
      deployedURL="https://saralaffin.github.io/responsive-website/"
    />
  </div>
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
#projects {
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
</style>
