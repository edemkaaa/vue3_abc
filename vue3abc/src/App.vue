<script>
import User from './components/Employee.vue'
export default {
  data() {
    return {
      hunters: [
        {
          id: 1,
          name: 'Edem',
          salary: 23000,
          age: 18
        },
        {
          id: 2,
          name: 'Elvin',
          salary: 13000,
          age: 17
        },
        {
          id: 3,
          name: 'Osman',
          salary: 64000,
          age: 19
        },
      ],
    }
  },
  components: {
    User
  }
}
</script>

<template>
<User :name="name" :salary="salary" :age="age"/>
</template>

<style scoped>
.employee{
padding: 60px;
color: #a200ff;
display: flex;
text-align: left;
}
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