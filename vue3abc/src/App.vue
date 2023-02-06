<script>
  export default{
    name:'App',
	data() {
		return {
      Text: 'page',
      href: 'page.html',
      attr: 'hi.png',
		name: 'Edem',
    surname: 'Asanov',
		group: 'I-1-21',
		}
	}
}
</script>

<template>
<div> 
  <a href="page.html">page</a>
    <p> Привет, меня зовут {{name}} я из группы {{group}} а моя фамилия {{ surname }} !</p>
 <img v-bind:src="attr">
 </div>
</template>

<style>
p {
  font-size: large;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  color: rgb(104, 62, 62);
  }
  </style>