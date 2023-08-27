<template>
  <section class="reviews">
    <img id="quotes" src="../assets/images/bg-quotes.png" alt="" />
    <div class="review">
      <p>
        Fylo has improved our team productivity by an order of magnitude. Since
        making the switch our team has become a well-oiled collaboration
        machine.
      </p>
      <div class="profiles">
        <img src="../assets/images/profile-1.jpg" alt="" />
        <div class="profile">
          <h2>Satish Patel</h2>
          <h1>Founter & CEO Huddle</h1>
        </div>
      </div>
    </div>
    <!--  -->
    <div class="review">
      <p>
        Fylo has improved our team productivity by an order of magnitude. Since
        making the switch our team has become a well-oiled collaboration
        machine.
      </p>
      <div class="profiles">
        <img src="../assets/images/profile-1.jpg" alt="" />
        <div class="profile">
          <h2>Satish Patel</h2>
          <h1>Founter & CEO Huddle</h1>
        </div>
      </div>
    </div>
    <div class="review">
      <p>
        Fylo has improved our team productivity by an order of magnitude. Since
        making the switch our team has become a well-oiled collaboration
        machine.
      </p>
      <div class="profiles">
        <img src="../assets/images/profile-1.jpg" alt="" />
        <div class="profile">
          <h2>Satish Patel</h2>
          <h1>Founter & CEO Huddle</h1>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Reviews",
};
</script>

<style>
.reviews {
  display: flex;
  gap: 1rem;
  align-items: center;
  justify-content: center;
  padding: 10rem 0;
  position: relative;
}

.review {
  background-color: hsl(219, 30%, 18%);
  width: 25rem;
  color: hsl(0, 0%, 100%);
  font-family: "Raleway", sans-serif;
  padding: 2.5rem 2rem;
}

.review p {
  font-weight: 400;
  font-size: 0.88rem;
  line-height: 1.5rem;
}

.profiles {
  margin-top: 1.5rem;
  display: flex;
  gap: 0.8rem;
}

.profiles img {
  width: 2rem;
  height: 2rem;
  border-radius: 50%;
}

.profile h2 {
  font-weight: 700;
  font-size: 0.8rem;
  letter-spacing: 1.5px;
}

.profile h1 {
  font-size: 0.6rem;
  font-weight: 400;
  margin-top: 0.4rem;
}

#quotes {
  position: absolute;
  top: 23%;
  left: 14%;
  z-index: -1;
}
</style>
