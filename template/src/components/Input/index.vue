<template>
	<form
		v-bind:action="action">
		<input 
			v-bind:type="type" 
			v-bind:name="name"
			/>
	</form>
</template>

<script>
export default {
	name: "SARUInput",
	data: function () {
		return {};
	},
	props: {},
	methods: {
		action: function () {
			return false;
		}
	}
}
</script>

<style scoped="">
@import "./index.css";
</style>
