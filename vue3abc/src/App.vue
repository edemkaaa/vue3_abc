<script>
  export default{
    name:'App',
	data() {
		return {
		name: 'Edem',
    surname: 'Asanov',
		group: 'I-1-21',
		}
	}
}
</script>

<template>
<div> 
    <h1> Привет, меня зовут {{name}} я из группы {{group}} а моя фамилия {{ surname }} !</h1>
  </div>
</template>