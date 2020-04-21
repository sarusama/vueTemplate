<template>
	<form
		v-bind:action="action">
		<input 
			v-bind:type="type" 
			v-bind:name="name"
			v-on:input="input"
			v-on:change="change"
			/>
	</form>
</template>

<script>
export default {
	name: "SARUInput",
	data: function () {
		return {};
	},
	props: {
		name: {
			type: String,
			default: ""
		},
		type: {
			type: String,
			default: "text"
		},
		maxlength: {
			type: Number,
			default: -1
		},
		value: {
			type: String,
			default: ""
		}
	},
	methods: {
		action: function () {
			return false;
		},
		input: function () {
			this.$emit("input");
		},
		change: function () {
			this.$emit("change");
		}
	}
}
</script>

<style scoped>
@import "./index.css";
</style>
