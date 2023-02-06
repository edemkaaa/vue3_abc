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
    date: '6'
	}
},
methods: {
show: function() {
alert(today);
},
slozheniye: function() {
alert(this.num1 + this.num2)
},
shom: function(){
    let date = this.dayOfWeek(this.date);
    // const dayOfWeekDigit = new Date().getDay();
    // let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
    alert(date);
  },
  dayOfWeek: function(date){
    let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
    return days[date -1];
  },
  shot: function(str){
  alert(str*str);
  },
  shot1: function(str1){
    alert(str1*str1)
  }
}
}
let today = new Date();
</script>

<template>
<div> 
  <a href="page.html">page</a>
    <p> Привет, меня зовут {{name}} я из группы {{group}} а моя фамилия {{ surname }} !</p>
    <img height="250" width="800" v-bind:src="attr">
    <p class="sc">Сумма {{num1+num2+num3}}.</p>
    <p class="sc">Сумма {{obj.x + obj.y +obj.z}}.</p>
    <button class="button button1" @click="show">Узнать дату кликом</button> <br> 
    <button class="button button2" @mouseenter="show"> Узнать дату навестись</button> 
    <button class="button" @mouseenter="shom">Узнать день недели навестить</button>
    <button class="button" @click="shom">Узнать день недели кликов</button>
{{ dayOfWeekDigit }}
    <button class="button" @click="shot(2)">Выведет квадрат числа 2</button>
    <button class="button" @click="shot1(3)">Выведет квадрат числа 3</button>
 </div>
</template>

<style>
p {
  font-size: large;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  color: rgb(104, 62, 62);
  }
  .button {
background-color: #efed73; /* yellow */
border-radius: 1cm;
color: black;
padding: 15px;
text-align-last: justify;
text-decoration: double;
display: flexbox;
font-size: 10px;
margin: 5px 2px;
cursor: cell;
}
  </style>