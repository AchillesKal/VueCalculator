<template>
  <div class="keyboard">
    <button>7</button>
    <button>8</button>
    <button>9</button>
    <button>X</button>
    <button>4</button>
    <button>5</button>
    <button>6</button>
    <button>-</button>
    <button>3</button>
    <button>2</button>
    <button>1</button>
    <button>+</button>
  </div>
</template>

<script>
export default {
  name: 'CalculatorKeyboard',
}
</script>

<style scoped>
.keyboard{
  display: grid;
  grid-template-columns: 25% 25% 25% 25%;
}

.keyboard button{
  height: 40px;
  border: 0;
  background-color: #FFF;
}
</style>
