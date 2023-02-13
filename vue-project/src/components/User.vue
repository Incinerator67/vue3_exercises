<script>
	export default {
		props: {
		name: String,
		surn: String
    },
	data() {return {name: 'name',surn: 'surname',}}
    }
</script>
<template>
	{{ name }}
	{{ surn }}
</template>