<script>
  export default{
    data() {
	return {
	}
},
methods: {

}
}
</script>

<template>
  <ul>
    <p :style="{color: 'green', fontSize: '30px', backgroundColor: 'yellow', fontStyle: 'italic', fontWeight: 'bold'}">
		text
	</p>
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