<script setup>
import catmeme3_a from '@/assets/images/catmeme3_a.jpg';
import catmeme3_b from '@/assets/images/catmeme3_b.jpg';
import whenAndWhere from '@/assets/images/whenandwhere.png';
</script>

<template>
	<section>
		<!-- Absolute path to /public folder -->
		<img src="/images/catmeme1_a.jpg" alt="" />
		<img src="/images/catmeme1_b.jpg" alt="" />
	</section>

	<section>
		<!-- Relative path to /assets folder -->
		<img src="@/assets/images/catmeme2_a.jpg" alt="" />
		<img src="@/assets/images/catmeme2_b.jpg" alt="" />
	</section>

	<section>
		<!-- Import asset into component -->
		<img v-bind:src="catmeme3_a" alt="" />
		<img :src="catmeme3_b" alt="" />
	</section>
	<div class="when-and-where">
		<!-- Import asset into component -->
		<img :src="whenAndWhere" alt="" />
	</div>
</template>

<style scoped>
section {
	display: grid;
	grid-template-columns: 1fr 1fr;
	padding: 10px;
	background: white;
	border-radius: 10px;
}
img {
	width: 100%;
}
</style>
