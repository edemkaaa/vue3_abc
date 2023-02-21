<script>
  export default{
    data() {
      return {
		selected: 'value1',
		options: ['Понедельник', 'Вторник', 'Среда','Четверг','Пятница','Суббота','Воскресенье'],
    days: '1',
    options1: ['1', '2', '3', '4', '5', '6', '7', '8', '9', '10', '11', '12', '13', '14', '15', '16', '17', '18', '19', '20', '21', '22', '23', '24', '25', '26', '27', '28', '29', '30',' 31'],
    month: 'Январь',
    options2: ['Январь', 'Февраль','Март', 'Апрель', 'Май','Июнь', 'Июль', 'Август', 'Сентябрь','Октябрь', 'Ноябрь', 'Декабрь'],
    years: '2023',
    options3: ['2001', '2002','2003', '2004', '2005','2006']
	}
},
methods: {

}
}
</script>

<template>
<ul>
	<select v-model="selected">
		<option v-for="option in options">{{ option }}</option>
	</select>
	<p>{{ selected }}</p>
  <br>
  <p class="button">Выберите день своего рождения</p>
  <br>
  <select v-model="days">
  <option v-for="option1 in options1">{{ option1 }}</option>
</select>
<br>
<select v-model="month">
  <option v-for="option2 in options2">{{ option2 }}</option>
</select>
<br>
<select v-model="years">
  <option v-for="option3 in options3">{{ option3 }}</option>
</select>
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