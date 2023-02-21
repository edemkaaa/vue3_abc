<script>
  export default{
  data() {
	return {
		arr: ['a', 'b', 'c'],
	}
},
methods: {
	add: function() {
		this.arr.push('xxx');
	},
  del: function() {
		this.arr.shift();
	},
  del1: function() {
		this.arr.pop();
	},
  splice: function(){
    this.arr.splice();
  },
  sort: function(){
    this.arr.sort();
  },
  reverse: function () {
    this.arr.reverse();
  },
}
  }
</script>

<template>
  <ul>
    <p v-for="elem in arr">
		{{ elem }}
	</p>
	<button @click="add">добавить</button>
  <button @click="del">удалить первую строку</button>
  <button @click="del1">удалить последнюю строку</button>
  <button @click="splice">удалить предпоследнюю строку</button>
  <button @click="sort">сортировать в обычном</button>
  <button @click="reverse">сортировать в обратном</button>
  </ul>
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