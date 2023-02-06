<script>
  export default{
    name:'App',
	data() {
		return {
		name: 'Edem',
		surname: 'Asanov',
		}
	}
}
</script>

<template>
<div> 
    <h1> Привет, меня зовут {{name}} я учусь в группе {{group}} </h1>
    <p> Введите корректное название :(</p>
  </div>
</template>