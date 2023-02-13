<script>
import User from './components/icons/User.vue'
	export default {
    components: {User}
    methods: {
      func() {alert('xxx');},
      handle() {this.$emit('show');}
  }
  }
</script>
<template>
  <User @show="func" />
  <button @click="handle">btn</button>
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
