<template>
<img src="https://image.freepik.com/free-vector/calculator-logo_10250-2607.jpg" alt="Logo"> <br>
Number 1: <input v-model.number="number1" type="text">
Number 2: <input v-model.number="number2" type="text"> <br>
<button v-on:click="add">Add</button>
<button v-on:click="subtract">Subtract</button>
<button v-on:click="multiply">Multiply</button>
<button v-on:click="divide">Divide</button> <br>
Result: {{ result }}
</template>

<script>
export default {
  name: 'App',
  data () {
    return {
      number1: 0,
      number2: 0,
      result: 0
    }
  },
  methods: {
    add () {
      this.result = this.number1 + this.number2
    },
    subtract () {
      this.result = this.number1 - this.number2
    },
    multiply () {
      this.result = this.number1 * this.number2
    },
    divide () {
      this.result = this.number1 / this.number2
      }
  }
}
</script>

<style>
#app{
font-family: Avenir, Helvetica, sans-serif;
text-align: center;
margin-top: 30px;
font-size: 190%;

}
</style>
