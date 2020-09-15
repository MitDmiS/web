<template>
  <div class="calculator">
    <calculator-display/>
    <div class="button-panel">
    <calculator-button
        v-for="item in array"
        :key="item"
    />
    </div>
  </div>
</template>

<script>
import CalculatorDisplay from "./CalculatorDisplay";
import CalculatorButton from "./CalculatorButton";
export default {
name: "Calculator",
  components: {CalculatorButton, CalculatorDisplay},
  data(){
  return{
    array:[
        0,1,2,3,4,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,22,23
    ]
  }
  }
}
</script>

<style scoped>
.calculator{
  display: flex;
  flex-direction: column;


  width: 345px;
  height: 550px;

  background: #C4C4C4;
  border-radius: 15px;
  box-shadow: 0 0 15px;
}

.button-panel{
  width: 285px;
  height: 410px;

  display: flex;
  flex-wrap: wrap;
  margin: auto;
}
</style>