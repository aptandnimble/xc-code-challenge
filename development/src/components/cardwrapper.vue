<template>
	<div>
		<draggable v-model="cards" v-bind="{group:'cardslots'}">
			<card
			v-for="(card, index) in cards"
			:key="index"
			:title="card.title"
			:image="card.image"
			:content="card.content"
			></card>
		</draggable>
	</div>
</template>

<script>

	import draggable from "../vuedraggable.js";
	import Card from './card'
	export default {
		components: {
			Card,
			draggable
		},
		data() {
			return {
				cards: []
			}
		},
		props: {
			data: {
				type: Array,
				required: true
			}
		},
		mounted() {
			this.cards = this.data
		}
	}
</script>

<style scoped lang="scss">
	@import '../assets/scss/_variables.scss';
	@import '../assets/scss/_core.scss';
	@import '../assets/scss/_card.scss';
</style>
