<script>
export default {
  data() {return {isAuth: true}},
  methods: {
    toggle: function() {this.isAuth = !this.isAuth;}
  }
</script>
<template>
  <button @click="toggle">toggle</button>
  <div v-if="isAuth">
		<p>+++</p>
		<p>+++</p>
	</div>
  <div v-else>Something Wrong</div>
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
