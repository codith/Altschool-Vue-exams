<template>
  <div class="counter">
    <h1 class="heading">Counter:{{ count }}</h1>

    <div class="btn-wrapper">
      <button @click="increment">+</button>

      <button @click="decrement">-</button>

      <button @click="reset">Reset</button>
    </div>
    <div>
      <input  type="number" v-model="value" />
      <button class="btn setvalue" @click="setValue(value)">Set Value</button>
    </div>
    
  </div>
</template>

<script>
import useCounter from "../composables/counter";

export default {
  setup() {
    const { count, increment, decrement, reset, setValue } = useCounter();

    return {
      count,
      increment,
      decrement,
      reset,
      setValue,
      value: 0,
    };
  },
};
</script>

<style scoped>
.counter {
  margin: 20px 0;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.heading {
  font-size: 3rem;
  padding-left: 6rem;
  color: #c19f68;
  text-align: center;
  font-weight: bolder;
  justify-content: center;
  margin-bottom: 16px;
  font-family: primaryFont;
}


input {
  width: 18%;
  padding: 0.3rem .5rem;
  font-size: 2rem;
  border-radius: 0.4rem;
}

button {
  font-size: 2rem;
  margin: 0.4em;
  padding: 0.4rem 1.2rem;
  background-color: #c19f68;
  box-shadow: 0 0.2rem 0.4rem rgba(0, 0, 0, 0.4);
  color: rgb(235, 231, 231);
  border: none;
  border-radius: 0.5rem;
  cursor: pointer;
  transition: all 0.3s;
}

button:hover {
  background-color: hsl(37, 63%, 80%);
  color: rgb(104, 100, 100);
  transform: translateY(-0.3rem);
}

@keyframes fadeIn {
  0% {
    opacity: 0;
  }
  100% {
    opacity: 1;
  }
}
</style>
