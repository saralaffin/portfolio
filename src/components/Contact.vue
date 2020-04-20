<template>
  <div id="contact">
    <h2>
      Keep in touch!
    </h2>
    <a href="Sara_Laffin_Resume.pdf" download>
      Resume
    </a>
    <p>I'm looking for full time work</p>
    <div class="contact-links">
      <a href="https://www.linkedin.com/in/saralaffin"
        ><i class="icon-linkedin"></i
      ></a>
      <a href="https://github.com/saralaffin"><i class="icon-github"></i></a>
    </div>
  </div>
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
}
.contact-links {
  display: flex;
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
