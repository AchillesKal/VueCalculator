<template>
  <div class="calculator">
    <div class="calculator-screen">
      <calculator-screen
        v-bind:screenText="screenText"
      ></calculator-screen>
    </div>
    <div class="calculator-keyboard">
       <calculator-keyboard
        v-on:number-press="onNumberPress"
        v-on:back-press="removeLastNumber"
       ></calculator-keyboard>
    </div>
  </div>
</template>

<script>
import CalculatorScreen from '@/components/CalculatorScreen.vue';
import CalculatorKeyboard from '@/components/CalculatorKeyboard.vue';

export default {
  name: 'Calculator',
  data: function () {
    return {
      screenText: "0"
    }
  },
  methods: {
    onNumberPress: function(number) {
      if(this.screenText.length <= 9){
        if(this.screenText.charAt(0) == "0"){
          this.screenText = this.screenText.substr(1);
        }
        this.screenText += number;
      }
    },
    removeLastNumber: function(){
      this.screenText =  this.screenText.slice(0, -1);
    }
  },
  components: {
    CalculatorScreen,
    CalculatorKeyboard
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
