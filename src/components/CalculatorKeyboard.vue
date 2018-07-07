<template>
  <div class="keyboard">
    <button>CE</button>
    <button>C</button>
     <button v-on:click="$emit('back-press')"><</button>
    <button>%</button>
    <button v-on:click="$emit('number-press', 7)">7</button>
    <button v-on:click="$emit('number-press', 8)">8</button>
    <button v-on:click="$emit('number-press', 9)">9</button>
    <button>X</button>
    <button v-on:click="$emit('number-press', 4)">4</button>
    <button v-on:click="$emit('number-press', 5)">5</button>
    <button v-on:click="$emit('number-press', 6)">6</button>
    <button>-</button>
    <button v-on:click="$emit('number-press', 3)">3</button>
    <button v-on:click="$emit('number-press', 2)">2</button>
    <button v-on:click="$emit('number-press', 1)">1</button>
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
