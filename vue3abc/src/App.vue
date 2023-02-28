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
    change(id, name, surn){
      this.users = this.users.map((user) => {
        if(user.id === id){
          user.name = name;
          user.surn = surn;
        }
        return user;
      });
    }
  }
}
</script>

<template>
<User v-for   ="user in users"
		:id     ="user.id"
		:name   ="user.name"
		:surn   ="user.surn"
		:key    ="user.id"
    @change="change"/>
</template>