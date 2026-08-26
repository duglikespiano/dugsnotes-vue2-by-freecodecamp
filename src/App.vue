<script setup>
/*
	const { createApp, ref } = Vue;
	createApp({
	  setup() {
	    const name = ref('Dug');
	    const emoji = ref('✌🏻');
	    return { name, emoji };
	  }
	}).mount('#app');
	*/
import { ref } from 'vue';
const name = ref('Dug');
const emoji = ref('✌🏻');
const year = ref('2014');
</script>

<template>
	<header>
		<span>{{ emoji }}</span>
	</header>

	<main>
		<h1>Hello, {{ name }}!</h1>
		<p>I'm about to learn <a href="https://vuejs.org/" target="_blank">Vue.js</a>!</p>
	</main>

	<footer>
		<p>&copy; {{ year }}</p>
	</footer>
</template>

<style scoped>
header span {
	font-size: 3rem;
}
main h1 {
	display: block;
}
main a {
	color: #42b883;
}
footer {
	position: fixed;
	bottom: 0;
	padding-bottom: 20px;
}
footer p {
	color: blue;
}
</style>
