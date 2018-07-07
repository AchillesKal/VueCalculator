<template>
  <div class="calculator">
    <div class="calculator-screen">
      <calculator-screen></calculator-screen>
    </div>
  </div>
</template>

<script>
import CalculatorScreen from '@/components/CalculatorScreen.vue';

export default {
  name: 'Calculator',
  components: {
    CalculatorScreen
  }
}
</script>

<style scoped>
.calculator{
  border: solid 1px #2e7e9c52;
  min-width: 350px;
  display: inline-block;
  background-color: #e8e8e8ad;
  box-shadow: 0 0 10px 1px #5f5f5f7a;
  min-height: 450px;
  padding: 5px;
  box-sizing: border-box;
}
</style>
