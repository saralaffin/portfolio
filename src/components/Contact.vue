<template>
  <article id="contact">
    <h2>
      Keep in touch!
    </h2>
    <p>
      I'm looking for front-end positions using React, but excited to apply my
      skill set to full-stack or back-end positions as well
    </p>
    <div class="contact-links">
      <a href="https://www.linkedin.com/in/saralaffin" target="_blank"
        ><i class="icon-linkedin"></i
      ></a>
      <a href="https://github.com/saralaffin" target="_blank"
        ><i class="icon-github"></i
      ></a>
      <a href="mailto:sarala@umich.edu"><i class="icon-envelope"></i></a>
    </div>
    <a href="Sara_Laffin_Resume.pdf" target="_blank">
      Resume
    </a>
  </article>
</template>

<script>
export default {
  name: "Contact",
};
</script>

<style scoped>
#contact {
  background-color: var(--white);
  display: flex;
  flex-direction: column;
  align-items: center;
}
h2 {
  color: var(--dark-blue);
}
p {
  padding-top: 2em;
  max-width: 600px;
  text-align: center;
  line-height: 2em;
}
.contact-links {
  display: flex;
  margin-bottom: 1vh;
}
.contact-links a {
  border-radius: 10vh;
  height: 10vh;
  width: 10vh;
  font-size: 4vh;
  margin: 1vh;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>
