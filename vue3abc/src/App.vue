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
    obj: {x: 5, y: 10, z: 15},
	}
},
methods: {
show: function() {
alert(today);
},
slozheniye: function() {
alert(this.num1 + this.num2)
}
}
}
let today = new Date();
</script>

<template>
  <button v-on:click="show">text</button>
<div> 
  <a href="page.html">page</a>
    <p> Привет, меня зовут {{name}} я из группы {{group}} а моя фамилия {{ surname }} !</p>
    <p class="sc">Сумма {{num1+num2+num3}}.</p>
    <p class="sc">Сумма {{obj.x + obj.y +obj.z}}.</p>
    <button class="button button1" @click="show">Узнать дату кликом</button> <br> 
    <button class="button button2" @mouseenter="show"> Узнать дату навестись</button> 
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