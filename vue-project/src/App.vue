<script>
export default {
  data() {return {users: [
			{
				id: 1,
				name: 'name1',
				salary: 100,
				age: 30,
			},
			{
				id: 2,
				name: 'name2',
				salary: 200,
				age: 40,
			},
			{
				id: 3,
				name: 'name3',
				salary: 300,
				age: 50,
			},
		],}},
  methods: {
    addItem: function() {
      removeItem: function(id) {this.users = this.users.filter((user) => {return user.id !== id;})}
    }
  }}
</script>
<template>
  <ul>
		<li v-for="user in users" :key="user.id">
			{{ user.name }}
			{{ user.surn }}
      <p>Salary</p>{{ user.salary }}
      <p>Age:</p>{{ user.age }}
			<button @click="removeItem(user.id)">remove</button>
		</li>
	</ul>
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
