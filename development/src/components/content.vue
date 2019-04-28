<template>
	<main id="main">
		<div class="column-wrapper">
			<cardwrapper :data="cards"></cardwrapper>
		</div>
	</main>
</template>

<script>
	import cardwrapper from './cardwrapper'
	import squareOne from '../assets/images/square-1.jpg'
	import squareTwo from '../assets/images/square-2.jpg'
	import squareThree from '../assets/images/square-3.jpg'
	export default {
		components: {
			cardwrapper
		},
		data() {
			return {
				cards: [
					{
						title: 'Introduction to Habitat',
						content: [
							'Sitecore Habitat is a range of sites demonstrating the capabilities of the Sitecore Experience Platform.',
							'The solution is built on the Sitecore Helix guidelines, which focuses on increasing productivity and quality in Sitecore projects.'
						],
						image: squareOne
					},
					{
						title: 'Modules',
						content: [
							'The Habitat example implementation has a range of modules which covers the basics of a Sitecore website.'
							],
						image: squareTwo
					},
					{
						title: 'Getting Started',
						content: [
							'Sitecore Helix a defined methodology with conventions and practices - Habitat is an example implementation available for your understanding.'
						],
						image: squareThree
					}
				]
			}
		}
	}
</script>

<style scoped lang="scss">
	@import '../assets/scss/_variables.scss';
	@import '../assets/scss/_core.scss';
	@import '../assets/scss/_card.scss';
</style>
