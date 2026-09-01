<script setup>
import { ref } from 'vue';
const quote = ref('First, solve the problem. Then, write the code');
const author = ref('John Johnson');
const href = ref('https://en.wikipedia.org/wiki/Undocumented_feature');

quote.value = "It's a feature, not a bug";
author.value = 'Unknown';
</script>

<template>
	<main>
		<section>
			<p>{{ quote }}</p>
			<a v-bind:href="href"
				><span>{{ author }}</span></a
			>
		</section>
		<button>Another!</button>
	</main>
</template>

<style scoped>
main {
	background: #ccd6d9;
	max-width: 90%;
	border-radius: 0 15px 0 15px;
	padding: 35px;
	display: flex;
	flex-direction: column;
	align-items: center;
	gap: 10px;
}

section {
	display: flex;
	width: 100%;
	flex-direction: column;
	gap: 10px;
	margin-bottom: 25px;
}

p {
	font-weight: bold;
	font-style: italic;
	font-size: 2rem;
	text-align: left;
}

p::before {
	content: '"';
}

p::after {
	content: '"';
}

span,
a {
	align-self: end;
	color: #406473;
}

span::before {
	content: '- ';
}

button {
	background: #406473;
	color: white;
	padding: 10px;
	border: 0;
	font-size: 1.2rem;
	border-radius: 0 5px 0 5px;
	font-weight: bold;
	margin-top: 20px;
	cursor: pointer;
	transition: transform 0.2s;
}
button:hover {
	transform: scale(1.05);
}
</style>
