<template>
	<svg
		xmlns="http://www.w3.org/2000/svg"
		:width="size"
		:height="size"
		viewBox="0 0 24 24"
		fill="none"
		v-if="type === 'bold'"
	>
		<path
			:fill="color"
			d="M18.68 13.978l-3.21-3.21-1.96-1.97a2.13 2.13 0 00-3.01 0l-5.18 5.18c-.68.68-.19 1.84.76 1.84h11.84c.96 0 1.44-1.16.76-1.84z"
		></path>
	</svg>
	<svg
		xmlns="http://www.w3.org/2000/svg"
		:width="size"
		:height="size"
		viewBox="0 0 24 24"
		fill="none"
		v-else-if="type === 'broken'"
	>
		<path
			:stroke="color"
			stroke-linecap="round"
			stroke-linejoin="round"
			stroke-miterlimit="10"
			:stroke-width="strokeWidth"
			d="M16.01 11.15L13.4 8.53c-.77-.77-2.03-.77-2.8 0l-6.52 6.52M19.92 15.05l-1.04-1.04"
		></path>
	</svg>
	<svg
		xmlns="http://www.w3.org/2000/svg"
		:width="size"
		:height="size"
		viewBox="0 0 24 24"
		fill="none"
		v-else-if="type === 'bulk'"
	>
		<path
			:fill="color"
			d="M15.48 10.77l-3.79 5.05H6.08c-.96 0-1.44-1.16-.76-1.84L10.5 8.8a2.13 2.13 0 013.01 0l1.97 1.97z"
			opacity=".4"
		></path>
		<path
			:fill="color"
			d="M17.92 15.82h-6.23l3.79-5.05 3.21 3.21c.67.68.19 1.84-.77 1.84z"
		></path>
	</svg>
	<svg
		xmlns="http://www.w3.org/2000/svg"
		:width="size"
		:height="size"
		viewBox="0 0 24 24"
		fill="none"
		v-else-if="type === 'linear'"
	>
		<path
			:stroke="color"
			stroke-linecap="round"
			stroke-linejoin="round"
			stroke-miterlimit="10"
			:stroke-width="strokeWidth"
			d="M19.92 15.05L13.4 8.53c-.77-.77-2.03-.77-2.8 0l-6.52 6.52"
		></path>
	</svg>
	<svg
		xmlns="http://www.w3.org/2000/svg"
		:width="size"
		:height="size"
		viewBox="0 0 24 24"
		fill="none"
		v-else-if="type === 'outline'"
	>
		<path
			:fill="color"
			d="M19.92 15.8c-.19 0-.38-.07-.53-.22l-6.52-6.52c-.48-.48-1.26-.48-1.74 0l-6.52 6.52c-.29.29-.77.29-1.06 0a.754.754 0 010-1.06L10.07 8a2.74 2.74 0 013.86 0l6.52 6.52c.29.29.29.77 0 1.06-.15.14-.34.22-.53.22z"
		></path>
	</svg>
	<svg
		xmlns="http://www.w3.org/2000/svg"
		:width="size"
		:height="size"
		viewBox="0 0 24 24"
		fill="none"
		v-else-if="type === 'twotone'"
	>
		<path
			:stroke="color"
			stroke-linecap="round"
			stroke-linejoin="round"
			stroke-miterlimit="10"
			:stroke-width="strokeWidth"
			d="M19.92 15.05L13.4 8.53c-.77-.77-2.03-.77-2.8 0l-6.52 6.52"
		></path>
	</svg>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
	name: 'ArrowUp2Icon',
	props: {
		type: {
			type: String,
			default: "linear"
		},
		size: {
			type: [String, Number],
			default: 24
		},
		color: {
			type: String,
			default: "currentColor"
		},
		strokeWidth: {
			type: String,
			default: "1.5"
		}
	}
});
</script>
