<script>
export default {
  data() {return {obj: {
			adone: true,
			selected:  false,
		}}},
  methods: {
	  setDone: function() {this.obj.hidden = false;}
  },
  power:{
    setDone2: function() {this.obj.hidden = true;}
  }
}
</script>
<template>
  <p :class="obj">Something Wrong</p>
  <button @click="setDone">text1</button>
  <button @click="setDone2">text2</button>
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
