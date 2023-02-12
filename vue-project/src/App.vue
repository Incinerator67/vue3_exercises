<script>
export default {
  data() {return {arr: ['x', 'y', 'z']}},
  methods: {
    toggle: function() {this.isAuth = !this.isAuth;}
  }
}
</script>
<template>
  	<p v-for="(elem, key) in arr">
		 <ul>{{ key+1 }}</ul> 
     {{ elem }}
	</p>
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
