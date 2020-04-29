<template>
  <article id="about">
    <h2>
      I've learned a lot over the past few months!
    </h2>
    <div class="content-container">
      <img
        src="../assets/GA13Feb_Linked-18.jpg"
        alt="Sara Laffin's profile picture"
      />
      <div class="text-container">
        <p>
          I've just graduated from a coding bootcamp, General Assembly, in
          Washington, DC. This portfolio showcases a few of my projects.
        </p>
        <p>
          With a Master's in engineering and a few years serving with
          AmeriCorps, I bring hard work and an analytical mind to every team.
        </p>
        <a href="Sara_Laffin_Resume.pdf" target="_blank">
          Resume
        </a>
      </div>
    </div>
  </article>
</template>

<script>
export default {
  name: "About",
};
</script>

<style scoped>
#about {
  background-color: var(--white);
  display: flex;
  flex-direction: column;
  align-items: center;
}
h2 {
  color: var(--dark-blue);
}
img {
  width: 25%;
  height: 25%;
  border-radius: 100%;
}
p {
  text-align: center;
  width: 80vw;
}

.content-container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.text-container {
  display: flex;
  flex-direction: column;
  align-items: center;
}
a {
  width: fit-content;
}
@media only screen and (min-width: 768px) {
  .content-container {
    flex-direction: row;
  }
  p {
    text-align: center;
    margin-bottom: 1.5em;
    padding: 0;
    width: 30vw;
  }
}
</style>
