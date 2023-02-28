<script>
export default{
data(){
  return{
		users: [
    {
				id: 1,
				name: 'edem',
				salary: 50000,
				age: 18,
			},
			{
				id: 2,
				name: 'elvin',
				salary: 12000,
				age: 17,
			},
			{
				id: 3,
				name: 'ilya',
				salary: 4300,
				age: 19,
			},
		]
  }
},
methods: {
  edit(user) {
    user.isEdit = true;
  },
  save(user) {
    user.isEdit = false;
  },
}
}
</script>

</template>
<template v-else>
  <input v-model="user.name">
  <input v-model="user.salary">
  <input v-model="user.age">
  <button class="button" @click="save(user)"> save
  </button>
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