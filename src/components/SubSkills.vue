<template>
  <div class="sub-skills">
    <i :class="icon"></i>
    <h3>
      {{ title }}
    </h3>
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
h3 {
  color: var(--dark-blue);
}
i {
  background-color: var(--dark-blue);
  color: var(--white);
  border-radius: 100%;
  height: 64px;
  width: 64px;
  font-size: 32px;
  margin: 8px;
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
    align-items: flex-end;
    padding-bottom: 2em;
  }
  p {
    padding: 1em 1em 1em 0;
    margin: 0;
    text-align: right;
    width: 488px;
  }
  i {
    margin-right: -64px;
    margin-bottom: -80px;
  }
}
</style>
