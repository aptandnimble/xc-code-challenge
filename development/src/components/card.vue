<template>
	<article>
		<div class="card">
			<img
			:src="image"
			>
			<h2>{{ title }}</h2>
			<p v-for="(p,index) in content" :key="index">{{ p }}</p>
			<ul class="actions">
				<li><a href="#" class="button" aria-label="Read more about Modules">Read more</a></li>
			</ul>
		</div>
	</article>
</template>

<script>
export default {
	props: {
		title: {
			type: String,
			required: true
		},
		content: {
			type: Array,
			required: true
		},
		image: {
			type: String,
			required: true
		}
	}
}
</script>

<style scoped lang="scss">

@import '../assets/scss/_variables.scss';
@import '../assets/scss/_core.scss';
@import '../assets/scss/_card.scss';

</style>
