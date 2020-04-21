<template>
  <div class="sub-skills">
    <i :class="icon"></i>
    <h4>
      {{ title }}
    </h4>
    <p>{{ content }}</p>
  </div>
</template>

<script>
export default {
  name: "SubSkills",
  props: {
    title: String,
    content: String,
    icon: String,
  },
};
</script>

<style scoped>
.sub-skills {
  background-color: var(--white);
  display: flex;
  flex-direction: column;
  align-items: center;
}
h2,
h4 {
  color: var(--dark-blue);
}
i {
  background-color: var(--dark-blue);
  color: var(--white);
  border-radius: 8vw;
  height: 8vw;
  width: 8vw;
  font-size: 4vw;
  margin: 1vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
p {
  text-align: center;
  padding-bottom: 2em;
}
@media only screen and (min-width: 992px) {
  .sub-skills {
    width: 25vw;
  }
  p {
    padding: 1em 2em;
    margin: 0;
  }
}
</style>
