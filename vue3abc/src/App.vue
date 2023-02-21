<script>
  export default{
    data() {
      return {
        language: '',
	}
},
methods: {

}
}
</script>

<template>
<ul>
  <p>Какой язык ваш родной?</p>
<input name="radio" type="radio" v-model="language" value="русский" @click="one">
<label for="">русский</label>
<br>
<input name="radio" type="radio" v-model="language" value="английский" @click="two">
<label for="">английский</label>
<br>
<input name="radio" type="radio" v-model="language" value="татарский" @click="three">
<label for="">татарский</label>
<br>
  Вы выбрали: {{ language }}
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