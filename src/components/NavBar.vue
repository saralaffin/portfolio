<template>
  <div class="navbar">
    <template v-for="section in sections">
      <a
        :key="section"
        :href="'#' + section"
        :class="{ isActive: section === activeSection }"
        >{{ titles[section] }}</a
      >
    </template>
  </div>
</template>

<script>
export default {
  name: "NavBar",
  data() {
    return {
      sections: ["about", "background", "skills", "projects", "contact"],
      titles: {
        about: "Intro",
        background: "My Story",
        skills: "Skills",
        projects: "Projects",
        contact: "Contact",
      },
      activeSection: "",
    };
  },
  mounted() {
    let observer = new IntersectionObserver(this.handler, {
      threshold: 0.1, //trying to fix a bug, "projects" doesn't highlight after scolling up from contact section
    });
    this.sections.forEach((section) => {
      observer.observe(document.getElementById(section));
    });
  },
  methods: {
    handler(entries) {
      for (const entry of entries) {
        const isVisible = entry.isIntersecting;

        if (isVisible) {
          this.activeSection = entry.target.id;
        }
      }
    },
  },
};
</script>

<style scoped>
.navbar {
  transform-origin: top left;
  transform: translateX(100vw) rotate(90deg);
  position: fixed;
  z-index: 1;
}
a:first-child {
  background-color: red;
}
a:nth-child(2) {
  background-color: orangered;
}
a:nth-child(3) {
  background-color: green;
}
a:nth-child(4) {
  background-color: blue;
}
a:nth-child(5) {
  background-color: blueviolet;
}
a {
  padding: 0.2em;
  opacity: 60%;
  border-top-right-radius: 0;
  border-top-left-radius: 0;
}
.isActive {
  opacity: 100%;
  padding-bottom: 0.5em;
}
</style>
