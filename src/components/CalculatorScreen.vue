<template>
  <div class="screen">
    {{ screenText }}
  </div>
</template>

<script>
export default {
  name: 'CalculatorScreen',
  props: ['screenText']
}
</script>

<style scoped>
.screen{
  height:50px;
  line-height: 50px;
  font-size: 50px;
  text-align: right;
  padding: 0 10px;
}
</style>
