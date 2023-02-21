<script>
  export default{
    data() {
      return {
		num: 0,
		res: 0,
    sum: 0,
    number1: 0,
    number2: 0,
    text1:'',
    text2:'',
    text:'',
	}
},
methods: {
	calc: function() {
		this.res = this.num ** 2;
	},
  summary: function() {
  this.sum = this.number1 + this.number2;
  }
}
}
</script>

<template>
  <ul>
    <p>{{ res }}</p>
	<input v-model="num">
	<button v-on:click="calc">work</button>
  <p>{{ sum }}</p>
	<input v-model="number1">
  <input v-model="number2">
	<button v-on:click="summary">sum</button>
  <p> {{ text }}</p>
  <input v-model="text1">
  <input v-model="text2">
  <button v-on:click="">text</button>
  </ul>
</template>

<style scoped>
.selected{
padding: 15px;
color: #fffc41;
display: flex;
text-align: center;
}
p.hidden{
  display: none;
}
  .button {
background-color: #fffc41; /* yellow */
border: none;
color: black;
padding: 15px;
text-align: center;
text-decoration: none;
display: inline-block;
font-size: 16px;
margin: 4px 2px;
cursor: pointer;
}
.styles{
  color: aquamarine;
  display: block;
  direction: rtl;
  border: 1ex;
}
.active{
  color: #000;
  background-color: aliceblue;
  margin: auto;
  stroke: #000;
}
  </style>