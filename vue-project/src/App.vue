<script>
export default {
  data() {return {name: 'Edem',surn: 'Osmanov',cost:'10',amount:'25'}},
  computed: {
    full: function() {return this.name + ' ' + this.surn;},
    price:function() {return this.cost * this.amount;}
  },
  methods: {
    change: function() {this.cost = '100',this.price = this.cost * this.amount;;}
  }
}
</script>
<template>
	<p>{{ name }}</p>
	<p>{{ surn }}</p>
	<p>{{ full }}</p>
  <p>{{ price }}</p>
  <button @click="change">change_cost</button>
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
