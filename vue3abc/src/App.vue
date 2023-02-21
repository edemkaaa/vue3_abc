<script>
  export default {

  data(){
  return{
    arr: [1, -2, 3, -4, 5],
  }
},
methods: {
}
}
</script>

<template>
  <ul>
    <template v-for="elem in arr">
    <li v-if="elem > 0 ">{{ elem }}</li>
    </template>
  </ul>
</template>

<style>
p {
  font-size: large;
  font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;
  color: rgb(104, 62, 62);
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
  </style>