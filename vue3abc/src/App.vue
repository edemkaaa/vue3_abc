<script>
  export default {
    data() {
	return {
		name: 'Edemkaaa',
    group: 'I-1-21',
    surname: 'Asanov',
    attr: 'hi.png',
    text: 'page',
		href: 'page.html',
    num: 5,
    num1: 1,
		num2: 2,
		num3: 3,
    arr1: ['x', 'y', 'z'], 
    arr2: [1, 2, 3], 
	}
}
  }
</script>

<template>
<div> 
  <a href="page.html">page</a>
  <p class="sc">Сумма {{num1+num2+num3}}.</p>
    <p> Привет, меня зовут {{name}} я из группы {{group}} а моя фамилия {{ surname }} !</p>
 <img v-bind:src="attr">
 </div>
</template>

<style>
p {
  font-size: large;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  color: rgb(104, 62, 62);
  }
  </style>