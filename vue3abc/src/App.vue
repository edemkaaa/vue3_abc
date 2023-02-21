<script>
  export default {
  data() {
	return {
		products: [
			{
				id: 1,
				name: 'product1',
			},
			{
				id: 2,
				name: 'product2',
			},
			{
				id: 3,
				name: 'product3',
			},
		]
	}
},
methods: {
}
}
</script>

<template>
  <ul>
    <p v-for="product in products" :key="products.id">
		{{ product.name }}
	</p>
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