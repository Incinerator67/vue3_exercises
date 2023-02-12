<script>
export default {
  data() {return {user1: '100$',user2: '200$',user3: '300$'}},
}
</script>
<template>
  	<ul>
      <li v-for="(elem,index) in user1">
        user1 - {{ elem }} - {{ index }}  
      </li>
      <li v-for="elem in user2">
        user2 - {{ elem }} - {{ index }} 
      </li>
      <li v-for="elem in user3">
        user3 - {{ elem }} - {{ index }} 
      </li>
    </ul>
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
