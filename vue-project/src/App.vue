<script>
export default {
  data() {return {checked: true}},
}
</script>
<template>
  <input type="checkbox" v-model="checked">
  <div v-if="checked == true"><p>{{ checked ? 'yes' : 'no' }}</p></div>
	<div v-else>{{ checked ? 'yes' : 'no' }}</div>
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
