<template>
  <div id="background">
    <h2>
      I'm a problem solver
    </h2>
    <div class="text-container">
      <p>
        I've always been drawn to fixing and creating. As a child, I enjoyed
        building things with my dad. In high school, I fell in love with modular
        origami. As you may be aware, any building endeavor comes with a set of
        problems to solve.
      </p>
      <p>
        I studied marine engineering in college, earning my Masters and
        Bachelors from the University of Michigan. The problem sets, labs, and
        projects were seemingly endless, but success came in the form of all
        A's, Summa Cum Laude.
      </p>
      <p>
        I've held a variety of roles in the marine engineering field, mainly in
        the form of internships. After studidying and working almost non-stop
        for 5 years, I had a new problem to solve: burn-out.
      </p>
      <p>
        Next, I tried something more hands-on. 'Sharpened a different saw', if
        you will. I spent 3 seasons with Americorps, mainly on chainsaw crews
        out in Colorado. Running a chainsaw, and leading crews, presented their
        own obstacles that helped me grow and solve problems in unimaginable
        ways.
      </p>
      <p>
        Now I'm returning to my engineering roots in the form of a software
        engineer! My dream is to continue to build (and fix) challenging
        projects. What solutions can I help you find?
      </p>
    </div>
  </div>
</template>

<script>
export default {
  name: "About",
  props: {
    msg: String,
  },
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
p {
  padding: 1em 2em;
}
.link-container {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}
a {
  margin: 0.2em;
}
</style>
