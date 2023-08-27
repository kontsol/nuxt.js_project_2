<template>
  <section class="intro">
    <div class="intro-image">
      <img src="../assets/images/illustration-intro.png" />
    </div>
    <div class="intro-content">
      <h1>All your files in one secure location, accessible anywhere</h1>
      <p>
        Fylo scores all your most important files in one secure location. Access
        them wherever you need, share and collaborate with friends family, and
        co-workers
      </p>
      <button>Get Started</button>
    </div>
  </section>
</template>

<script>
export default {
  name: "Intro",
};
</script>

<style>
.intro {
  display: grid;
  place-items: center;
  font-family: "Raleway", sans-serif;
}

.intro-image {
  display: grid;
  place-items: center;
}

.intro-image img {
  width: 90%;
}

.intro-content {
  display: grid;
  place-items: center;
  text-align: center;
  color: hsl(0, 0%, 100%);
}

.intro-content h1 {
  font-size: 2rem;
  width: 40rem;
  line-height: 3.2rem;
  font-weight: 700;
}

.intro-content p {
  font-weight: 400;
  width: 36rem;
  font-size: 1.2rem;
  line-height: 1.9rem;
  margin-top: 2rem;
}

.intro-content button {
  text-align: center;
  padding: 1rem 5.5rem;
  font-size: 1.1rem;
  border-radius: 2rem;
  margin-top: 2rem;
  font-weight: 700;
  background-color: hsl(176, 68%, 64%);
  color: hsl(0, 0%, 100%);
  transition: all 0.3s ease-in;
}

.intro-content button:hover {
  background-color: hsl(198, 60%, 50%);
}

@media (max-width: 425px) {
  .intro-image img {
    margin-top: 2rem;
    width: 70%;
  }
}
</style>
