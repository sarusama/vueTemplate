<template>
	<div
		class="template-image">
		<img
			class="template-image-main"
			v-bind:src="src"
			v-bind:alt="alt"
			/>
	</div>
</template>

<script>
export default {
	name: "SARUImage",
	data: function () {
		return {};
	},
	props: {
		src: {
			type: String,
			default: ""
		},
		alt: {
			type: String,
			default: ""
		}
	}
}
</script>

<style scoped>
@import "./index.css";
</style>
