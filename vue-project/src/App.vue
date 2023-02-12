<script>
export default {
  data() {age: 25},

  
}
</script>
<template>
	<p v-if="age === 19 || age === 25">
		молодой человек
	</p>
  <p v-else-if="age >= 26">Мужчина</p>
  <p v-else>подросток</p>

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
