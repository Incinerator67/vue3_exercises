<script>
export default {
  data() {return {date:'10'},
  methods: {
	show: function() {
    let text = this.cape(this.date);
    alert(this.text);
  },
  cape: function(str) {return str[0].toUpperCase() + str.slice(1);}
}
}
</script>
<template>
<div>{{ 
<template>
  <button @mouseover="show">text</button>
</template> 
}}</div> 
</template>

<style scoped>
header {
  line-height: 1.5;
}

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
