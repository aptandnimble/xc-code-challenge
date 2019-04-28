<template>
	<div id="carousel-wrapper">
		<picture>
			<source srcset="../assets/images/slide-1.webp" type="image/webp">
			<source srcset="../assets/images/slide-1.jpg" type="image/jpeg">
			<img src="../assets/images/slide-1.jpg" alt="Sitecore Rocks!">
		</picture>
	</div>
</template>
<script>
export default {
	components: {
	}
}
</script>

<style scoped lang="scss">
	#carousel-wrapper img {
		width:100%;
	}
</style>
