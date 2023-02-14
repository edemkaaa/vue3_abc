<script>
  export default {
    data() {
	return {
		name: 'Edemkaaa',
    group: 'I-1-21',
    surname: 'Asanov',
    attr: 'hi.png',
    text: 'page',
    text1: 'edddem',
		href: 'page.html',
    num: 5,
    num1: 1,
		num2: 2,
		num3: 3,
    arr1: ['x', 'y', 'z'], 
    arr2: [1, 2, 3],
    obj: {x: 5, y: 10, z: 15},
    date: '6',
    cost: '1550',
    amount: '90',
    visible: true,
    visible1: false,
    hidden: true,
    hidden1: false,
	}
},
computed: {
	price: function() {
		return this.cost *  this.amount;
	}
},
methods: {
show: function() {
alert(today);
},
slozheniye: function() {
alert(this.num1 + this.num2)
},
hide: function() {
		this.visible = false;
	},
  hide2: function() {
		this.visible = true;
	},
shom: function(){
    let date = this.dayOfWeek(this.date);
    // const dayOfWeekDigit = new Date().getDay();
    // let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
    alert(date);
  },
  shor: function(){
    alert(new Date().toLocaleDateString());
},
  dayOfWeek: function(date){
    let days = ['Понедельник', 'Вторник', 'Среда', 'Четверг', 'Пятница', 'Суббота', 'Воскресенье']
    return days[date -1];
  },
  change: function(){
		this.text1 = 'edem';
	},
  change2: function(){
    this.text1 = 'asanov'
  },
  change3: function(){
    this.cost = '50'
  },
}
}
let today = new Date();
</script>

<template>
<div> 
  <a href="page.html">page</a>
    <p> Привет, меня зовут {{name}} я из группы {{group}} а моя фамилия {{ surname }} !</p>
    <p class="sc">Сумма {{num1+num2+num3}}.</p>
    <p class="sc">Сумма {{obj.x + obj.y +obj.z}}.</p>
    <p> {{ text1 }} </p>
    <p> {{ cost }} </p>
    <p> {{ amount }} </p>
    <p> {{ price }} </p>
    <button class="button button1" @click="show">Узнать дату кликом</button> <br> 
    <button class="button button2" @mouseenter="show"> Узнать дату навестись</button> 
    <button class="button" @mouseenter="shom">Узнать день недели навестить</button>
    <button class="button" @click="shom">Узнать день недели кликов</button>
    <button @click="change">edem</button>
    <button @click="change2">asanov</button>
    <button @click="change3">Меняем значение cost на 50</button>
    <button @click="hide">Убрать абзац</button>
	<p v-if="visible">text</p>
    <button @click="hide2">Вернуть абзац</button>
	  <p v-if="visible">text</p>
    <a class="inline-link-1" href="https://github.com/edemkaaa" onclick="event.preventDefault()"> Не сработает по клику</a>
    <a @click.once="shor"> Сработает один раз</a>
    <p v-if="visible">Показан</p>
    <p v-if="visible1">Не показан</p>
    <p v-if="hidden">Edem</p>
    <p v-if="!hidden1">Asanov</p>
    <p v-if="visible">text</p>
{{ dayOfWeekDigit }}
 <img v-bind:src="attr">
 </div>
</template>

<style>
p {
  font-size: large;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  color: rgb(104, 62, 62);
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
  </style>