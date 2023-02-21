<script>
  export default{
    data() {
      return {
        isDisabled: true,
        isDisabled1: true,
	}
},
methods: {
  toggle: function () {
    this.isDisabled = false;
  },
  toggle1: function () {
    this.isDisabled1 = false;
  },
}
}
</script>

<template>
<ul>
	<button v-bind:disabled="isDisabled">btn</button>
	<button v-bind:disabled="isDisabled">btn</button>
  <button class="button" @click="toggle">btn</button>
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