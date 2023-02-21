<script>
export default{
data(){
  return{
    newItem: '',
		items: ['a', 'b', 'c', 'd', 'e'],
  }
},
methods: {
  addItem: function() {
		this.items.push(this.newItem);
	},
  addItem1: function () {
    this.items.unshift(this.newItem);
  }
}
}
</script>

<template>
<ul>		
    <li v-for="(item, index) in items" :key="index">
			{{ item }}
		</li>
    <input v-model="newItem">
	<button @click="addItem">В конец</button>
	<button @click="addItem1">В начало</button>
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