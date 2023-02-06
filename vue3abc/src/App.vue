<script>
  export default{
    name:'App',
	data() {
		return {
      num: 5,
      num: 1,
      num: 2,
      num: 3,
      var1: 1,
      var2: 2,
      Text: 'page',
      href: 'page.html',
      attr: 'hi.png',
		name: 'Edem',
    surname: 'Asanov',
		group: 'I-1-21',
		}
	}
}
</script>

<template>
  {{ var1 + var2 }}
<div> 
  <a href="page.html">page</a>
    <p> Привет, меня зовут {{name}} я из группы {{group}} а моя фамилия {{ surname }} !</p>
 <img v-bind:src="attr">
 <p>{{ num1 + num2 + num3 }}</p>
 </div>
</template>

<style>
p {
  font-size: large;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  color: rgb(104, 62, 62);
  }
  </style>