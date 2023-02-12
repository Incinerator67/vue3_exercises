<script>
export default {
  data() {return {isAdmin: true}},
  methods: {
    toggle: function() {this.isAdmin = false;}
  }
  
}
</script>
<template>
  <button @click="toggle">toggle</button>
	<p v-if="isAdmin">Something Wrong</p>
  <p v-else>Something Wrong 2</p>
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
