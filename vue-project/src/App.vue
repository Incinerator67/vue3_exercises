<script>
  import User from './components/icons/User.vue'
  export default {components: {User},
      data() {return {
        users: [
          {
            id: 1,
            name: 'name1',
            surn: 'surn1'
          },
          {
            id: 2,
            name: 'name2',
            surn: 'surn2'
          },
          {
            id: 3,
            name: 'name3',
            surn: 'surn3'
          },
        ],
      }
    },
  methods: {
    add(name, surn) {
      let id = this.users.length + 1;
      this.users.push({
        id,
        name,
        surn
      });
    }
  }
  }
</script>
<template>
 <User Form @add="add" />
</template>
<style scoped>
header {line-height: 1.5;}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
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
