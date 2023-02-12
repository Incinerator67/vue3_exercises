<script>
export default {
  data() {return {	choice: 'my favorite program languege - is '}},
}
</script>
<template>
  <input name="radio" type="radio" v-model="choice" value="v1">
    <p>{{ arr }}PHP</p>
  <input name="radio" type="radio" v-model="choice" value="v2">
    <p>{{ arr }}C#</p>
  <input name="radio" type="radio" v-model="choice" value="v3">
    <p>{{ arr }}Assembler</p>
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
