<script>
  export default{
    data() {
      return {
        lang: [],
	}
},
methods: {

}
}
</script>

<template>
<ul>
	<input type="checkbox" v-model="lang" value="python">
  <label>python</label>
	<input type="checkbox" v-model="lang" value="jango">
  <label>jango</label>
	<input type="checkbox" v-model="lang" value="c++">
  <label>c++</label>
  <ul>
  <li v-for="elem in lang">{{ elem }}</li>
</ul>
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