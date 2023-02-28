<script>
export default{
data(){
  return{
		users: [
    {
				id: 1,
				name: 'edem',
				salary: 100,
				age: 18,
			},
			{
				id: 2,
				name: 'elvin',
				salary: 200,
				age: 17,
			},
			{
				id: 3,
				name: 'ilya',
				salary: 300,
				age: 19,
			},
		]
  }
},
methods: {
	removeItem: function(id) {
		this.users = this.users.filter((user) => {
			return user.id !== id;
		})
	}
}
}
</script>

<template>
	<ul>
		<li v-for="user in users" :key="user.id">
			{{ user.name }} {{ user.salary }} {{ user.age }} 
      <button class="button" @click="removeUser(user.id)">remove</button>
		</li>
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