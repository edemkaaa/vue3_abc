<script>
export default{
data(){
  return{
  text1: ' ',
  text2: ' '
  }
},
methods: {
}
}
</script>

<template>
<input class="text-field__input" v-model="text1" v-on:keyup.enter="submit">
<p>{{ text1 }}</p>
<br>
<a href="#" class="inline-link-1" v-on:keyup.ctrl="sub">text2</a>
<p ></p>
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