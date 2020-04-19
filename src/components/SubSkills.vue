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
  border-radius: 10vh;
  height: 10vh;
  width: 10vh;
  font-size: 4vh;
  margin: 1vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
p {
  text-align: center;
  padding: 1em;
}
</style>
