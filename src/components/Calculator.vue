<template>
  <div class="calculator">
    This is the calculator
  </div>
</template>

<script>
export default {
  name: 'Calculator',
  props: {
    msg: String
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
  min-height: 400px;
}
</style>
