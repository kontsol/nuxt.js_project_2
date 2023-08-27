<template>
  <section class="early-access">
    <div class="early-access-content">
      <h1>Get early access today</h1>
      <p>
        It only takes a minute to sign up and our free starter tier is extremely
        generous. If you have any questions, our support team would be happy to
        help you.
      </p>
      <div class="search-button">
        <input v-model="inputValue" type="text" />
        <button @click="handleButtonClick">Get started for free</button>
      </div>
      <p v-if="showMessage" class="error-message">
        Please enter a valid email address
      </p>
    </div>
  </section>
</template>

<script>
export default {
  name: "EarlyAccess",
  data() {
    return {
      inputValue: "",
      showMessage: false,
    };
  },
  methods: {
    handleButtonClick() {
      if (this.inputValue.trim() === "") {
        this.showMessage = true;
      } else {
        this.showMessage = false;
      }
    },
  },
};
</script>

<style>
.early-access {
  display: grid;
  place-items: center;
  font-family: "Raleway", sans-serif;
  color: hsl(0, 0%, 100%);
  position: relative;
}

.early-access-content {
  padding: 2.8rem 5.5rem;
  width: 50%;
  display: grid;
  place-items: center;
  background-color: hsl(219, 30%, 18%);
}

.early-access-content h1 {
  font-weight: 700;
  font-size: 2rem;
}

.early-access-content p {
  width: 90%;
  font-size: 0.9rem;
  margin-top: 1.8rem;
  text-align: center;
  line-height: 1.4rem;
}

.search-button {
  margin-top: 2rem;
  display: flex;
  align-items: center;
  gap: 1rem;
}

.search-button input {
  width: 30rem;
  height: 3rem;
  border-radius: 26px;
  outline: none;
  text-align: left;
  padding-left: 1rem;
  border: none;
}

.search-button button {
  width: 13rem;
  height: 3rem;
  text-align: center;
  font-weight: 700;
  color: hsl(0, 0%, 100%);
  background-color: hsl(176, 68%, 64%);
  border: none;
  border-radius: 26px;
  transition: all 0.3s ease-in;
}

.search-button button:hover {
  background-color: hsl(198, 60%, 50%);
}

.error-message {
  color: red;
  position: absolute;
  top: 78% !important;
  left: 4% !important;
}

@media (max-width: 425px) {
  .early-access-content {
    display: block;
  }
  .early-access {
    display: block;
  }
}
</style>
