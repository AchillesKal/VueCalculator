<template>
  <div class="keyboard">
    <button>CE</button>
    <button>C</button>
    <button><</button>
    <button>%</button>
    <button v-on:click="numberPress(7)">7</button>
    <button v-on:click="numberPress(8)">8</button>
    <button v-on:click="numberPress(9)">9</button>
    <button>X</button>
    <button v-on:click="numberPress(4)">4</button>
    <button v-on:click="numberPress(5)">5</button>
    <button v-on:click="numberPress(6)">6</button>
    <button>-</button>
    <button v-on:click="numberPress(3)">3</button>
    <button v-on:click="numberPress(2)">2</button>
    <button v-on:click="numberPress(1)">1</button>
    <button>+</button>
    <button>^</button>
    <button v-on:click="$emit('number-press', 0)">0</button>
    <button>,</button>
    <button>=</button>
  </div>
</template>

<script>
export default {
  name: 'CalculatorKeyboard',
  methods: {
  }
}
</script>

<style scoped>
.keyboard{
  padding-top: 10px;
  display: grid;
  grid-template-columns: 25% 25% 25% 25%;
}

.keyboard button{
  height: 40px;
  border: 0;
  background-color: #FFF;
  margin: 3px;
}
</style>
