<script setup>
/*
CHALLENGE: Create a Ref to house "https://vuejs.org/"
           and bind the Ref to our anchor tag's href attribute.
           Use shorthands if you want/can!
*/
import { ref } from 'vue';
const href = ref('https://vuejs.org/');
</script>

<template>
	<footer>
		<p>Learn more about me at <a target="_blank" :href>vuejs.org</a></p>
	</footer>
</template>

<style scoped>
footer {
	margin-top: 35px;
	font-size: 0.8rem;
}

a {
	color: #40b883;
}
</style>
