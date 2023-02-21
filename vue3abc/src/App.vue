<script>
  export default{
    data() {
      return {
		selected: 'value1', // значение по умолчанию
	}
},
methods: {

}
}
</script>

<template>
<ul>
  <p>В каком городе вы живете?</p>
	<select v-model="selected">
		<option>Симферополь</option>
		<option>Евпатория</option>
		<option>Феодосия</option>
	</select>
	<p>{{ selected }}</p>
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