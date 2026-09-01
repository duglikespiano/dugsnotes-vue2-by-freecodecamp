<script setup>
import { ref } from 'vue';
const year = ref('2025');
const href = ref('http://scrimba.com');
year.value = '2014';
</script>

<template>
	<footer>
		Created by <a v-bind:href="href"><span>Professor Pickle</span></a> &copy; {{ year }}
	</footer>
</template>

<style scoped>
footer {
	position: fixed;
	margin: 0 auto;
	bottom: 0;
	text-align: center;
	color: #ccd6d9;
	padding-bottom: 20px;
}

span {
	font-family: cursive;
}

a {
	color: white;
}
</style>
