<script>
export default {
  data: () => ({
    counter: 0,
  }),
  methods: {
    increment() {
      this.counter++;
    },
    decrease() {
      this.counter--;
    },
    reset() {
      this.counter = 0;
    },
  },
};
</script>

<template>
  <div class="container">
    <img src="./assets/logo.svg" alt="logo vue" width="125" height="125" />
    <small>
      <h1>Hello World from VUE.js!</h1>
    </small>
    <hr />

    <h2>Counter: {{ counter }}</h2>
    <button @click="increment()">+1</button>
    <button @click="decrease()">-1</button>
    <button @click="reset()">Reset</button>
  </div>
</template>

<style scoped>
.container {
  text-align: center;
}

small {
  color: #666;
  font-weight: bolder;
}

h2 {
  font-weight: bolder;
  color: #fff;
  font-size: 2.5rem;
}

button {
  cursor: pointer;
  font-size: 1.5rem;
  margin: 0px 6px;
  border-radius: 7px;
}
</style>
