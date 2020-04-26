<template>
  <article id="background">
    <h2>
      I'm a problem solver
    </h2>
    <div class="text-container">
      <p>
        I've always been drawn to fixing and creating. As a child, I enjoyed
        <b>building</b> things with my dad. In high school, I fell in love with
        modular origami.
      </p>
      <i class="icon-wrench"></i>
      <p>
        I studied marine engineering in college, earning my Masters and
        Bachelors from the University of Michigan.
        <b>Academic achievement</b> came in the form of all A's, Summa Cum
        Laude.
      </p>
      <i class="icon-book"></i>
      <p>
        I've held a variety of roles in the <b>marine engineering</b> field,
        mainly in the form of internships. After studidying and working almost
        non-stop for 5 years, I had a new problem to solve: burn-out.
      </p>
      <i class="icon-anchor"></i>
      <p>
        Next, I tried something more hands-on. 'Sharpened a different saw', if
        you will. I spent 3 seasons on conservation crews out in Colorado.
        Running a chainsaw, and <b>leading crews</b>, presented their own
        obstacles that helped me grow and solve problems in unimaginable ways.
      </p>
      <i class="icon-leaf"></i>
      <p>
        Now I'm returning to my engineering roots in the form of a software
        engineer! My dream is to continue to build (and fix) challenging
        projects. What <b>solutions</b> can I help you find?
      </p>
      <i class="icon-lightbulb"></i>
    </div>
  </article>
</template>

<script>
export default {
  name: "Background",
};
</script>

<style scoped>
#background {
  background-color: var(--dark-blue);
  display: flex;
  flex-direction: column;
  align-items: center;
}
h2 {
  color: var(--white);
  opacity: 1;
}
.text-container {
  text-align: center;
  margin-top: 4vh;
  margin-bottom: 10vh;
  color: var(--white);
}
.link-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
a {
  margin: 0.2em;
}
@media only screen and (min-width: 992px) {
  b {
    font-size: 24px;
  }
  p {
    width: 588px;
    padding-left: 16px;
    margin: 0;
    text-align: left;
  }
  p:first-child {
    margin-left: 80px;
  }
  .text-container {
    width: 668px;
    display: flex;
    flex-wrap: wrap;
  }
  i {
    background-color: var(--white);
    color: var(--dark-blue);
    border-radius: 100%;
    height: 64px;
    width: 64px;
    font-size: 32px;
    margin: 8px;
    margin-top: -64px;
    display: flex;
    justify-content: center;
    align-items: center;
  }
}
</style>
