<template>
  <div class="button">

  </div>
</template>

<script>
export default {
name: "CalculatorButton"
}
</script>

<style scoped>
.button{
  width: 60px;
  height: 60px;

  background: #fff;
  border-radius: 15px;
  margin: auto;
  box-shadow: 0 0 10px;
}

.button:hover{
  background: #ccc;
  box-shadow: 0 0 20px;
}

.button:active{
  background: #ccc;
  box-shadow: 0 0 15px;
  transform: translateY(3px);
}
</style>