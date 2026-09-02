<script setup>
import { ref } from 'vue';
const title = ref('Quote Generator');

title.value = 'Programming Quotes';
</script>

<template>
	<header>
		<h1>{{ title }}</h1>
	</header>
</template>

<style scoped>
header {
	color: #ccd6d9;
	margin-bottom: 25px;
}
</style>
