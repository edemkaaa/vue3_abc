<script>
import User from './components/Employee.vue'
import userform from './components/userform.vue'
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
    User, userform
  },
  methods: {
    add(name, surn){
      let id = this.users.length + 1;
      this.users.push({
        id, name, surn
      });
    }
  }
}
</script>

<template>
<userform @add="add"/>
</template>

<style scoped>
header {
  line-height: 1.5;
}
.logo {
  display: block;
  margin: 0 auto 2rem;
}
@media (min-width: 1024px) {
  .header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }
  .logo {
    margin: 0 2rem 0 0;
  }
  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>