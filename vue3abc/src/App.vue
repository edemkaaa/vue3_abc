<script>
import User from './components/Employee.vue'
export default {
  data() {
    return {
      users: [
        {
          id: 1,
          name: 'Edem',
          surn: 'Asanov'
        },
        {
          id: 2,
          name: 'Elvin',
          surn: 'Nikolayenko'
        },
        {
          id: 3,
          name: 'Edem',
          surn: 'Seytumerov'
        },
      ],
    }
  },
  components: {
    User
  },
  methods: {
    remove(id) {
      this.users = this.users.filter((user) => {
        return user.id !== id;
      })
    }
  }
}
</script>

<template>
<User v-for   ="user in users"
		:id     ="user.id"
		:name   ="user.name"
		:surn   ="user.surn"
		@remove ="remove"
		:key    ="user.id"/>
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