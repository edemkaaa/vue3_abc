<script>
  export default{
    data() {
	return {
    visible: true,
		style: {
			hidden: true,
		},
	}
},
methods: {
setone:function(){
  this.styles.hidden = false;
},
setTwo: function(){
  this.styles.hidden = true;
},
  toggle: function () {
    this.visible = !this.visible;
  }
}
}
</script>

<template>
  <ul>
<button class="selected" @click="toggle">toggle</button>
<p class="button" v-if="visible">Edem</p>
<p :class="styles">Conclave</p>
<button class="button" @click="setone">visible</button>
<button class="button" @click="setTwo">hide</button>
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
  </style>