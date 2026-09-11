<script setup>
import src from '@/assets/product_image.jpg';
</script>

<template>
	<main>
		<h1>Cat Enthusiast's Box</h1>

		<!-- PRODUCT IMAGE START -->
		<img v-bind:src="src" alt="cat box" />
		<!-- PRODUCT IMAGE END -->

		<p>
			Treat your feline friend to the purr-fect surprise with this Cat Enthusiast's Box! Filled with catnip toys, tasty treats,
			and a scratching pad, this box will keep your kitty entertained for hours. Whether they're a curious kitten or a majestic
			senior, they'll adore the goodies inside. Give your cat the royal treatment they deserve!
		</p>

		<button>Add to Cart</button>
	</main>
</template>

<style scoped></style>
