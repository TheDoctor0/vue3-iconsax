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
			d="M17.45 17.302c-1.68 0-3.23-.79-4.24-2.18-.24-.33-.17-.8.16-1.05s.8-.17 1.05.16c.73.99 1.83 1.56 3.03 1.56 2.09 0 3.8-1.7 3.8-3.8 0-2.1-1.7-3.8-3.8-3.8-1.42 0-2.76.76-3.49 1.97l-2.65 4.41c-1 1.67-2.83 2.7-4.77 2.7a5.31 5.31 0 0 1-5.3-5.3c0-2.92 2.38-5.3 5.3-5.3 1.68 0 3.23.79 4.24 2.18.24.33.17.8-.16 1.05a.75.75 0 0 1-1.05-.16c-.72-.97-1.82-1.54-3.02-1.54-2.09 0-3.8 1.7-3.8 3.8 0 2.1 1.7 3.8 3.8 3.8 1.42 0 2.76-.76 3.49-1.97l2.65-4.41c1-1.67 2.83-2.7 4.77-2.7 2.92 0 5.3 2.38 5.3 5.3s-2.39 5.28-5.31 5.28Z"
			:fill="color"
		></path>
		<path
			d="M6.5 14a2 2 0 1 0 0-4 2 2 0 0 0 0 4ZM17.5 14a2 2 0 1 0 0-4 2 2 0 0 0 0 4Z"
			:fill="color"
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
			d="M20 15.77c-.73.49-1.6.78-2.54.78-1.5 0-2.81-.74-3.64-1.87M10.18 9.32a4.474 4.474 0 0 0-3.64-1.87c-2.51 0-4.55 2.04-4.55 4.55s2.04 4.55 4.55 4.55c1.69 0 3.26-.89 4.13-2.34L12 12l1.32-2.21a4.821 4.821 0 0 1 4.13-2.34C19.96 7.45 22 9.49 22 12"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
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
			opacity=".4"
			d="M17.45 17.302c-1.68 0-3.23-.79-4.24-2.18-.24-.33-.17-.8.16-1.05s.8-.17 1.05.16c.73.99 1.83 1.56 3.03 1.56 2.09 0 3.8-1.7 3.8-3.8 0-2.1-1.7-3.8-3.8-3.8-1.42 0-2.76.76-3.49 1.97l-2.65 4.41c-1 1.67-2.83 2.7-4.77 2.7a5.31 5.31 0 0 1-5.3-5.3c0-2.92 2.38-5.3 5.3-5.3 1.68 0 3.23.79 4.24 2.18.24.33.17.8-.16 1.05a.75.75 0 0 1-1.05-.16c-.73-.99-1.83-1.56-3.03-1.56-2.09 0-3.8 1.7-3.8 3.8 0 2.1 1.7 3.8 3.8 3.8 1.42 0 2.76-.76 3.49-1.97l2.65-4.41c1-1.67 2.83-2.7 4.77-2.7 2.92 0 5.3 2.38 5.3 5.3s-2.38 5.3-5.3 5.3Z"
			:fill="color"
		></path>
		<path
			d="M6.5 14a2 2 0 1 0 0-4 2 2 0 0 0 0 4ZM17.5 14a2 2 0 1 0 0-4 2 2 0 0 0 0 4Z"
			:fill="color"
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
			d="M10.18 9.32a4.474 4.474 0 0 0-3.64-1.87c-2.51 0-4.55 2.04-4.55 4.55s2.04 4.55 4.55 4.55c1.69 0 3.26-.89 4.13-2.34L12 12l1.32-2.21a4.821 4.821 0 0 1 4.13-2.34C19.96 7.45 22 9.49 22 12s-2.04 4.55-4.55 4.55c-1.5 0-2.81-.74-3.64-1.87"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
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
			d="M17.45 17.302c-1.68 0-3.23-.79-4.24-2.18-.24-.33-.17-.8.16-1.05s.8-.17 1.05.16c.73.99 1.83 1.56 3.03 1.56 2.09 0 3.8-1.7 3.8-3.8 0-2.1-1.7-3.8-3.8-3.8-1.42 0-2.76.76-3.49 1.97l-2.65 4.41c-1 1.67-2.83 2.7-4.77 2.7a5.31 5.31 0 0 1-5.3-5.3c0-2.92 2.38-5.3 5.3-5.3 1.68 0 3.23.79 4.24 2.18.24.33.17.8-.16 1.05a.76.76 0 0 1-1.05-.16c-.73-.99-1.83-1.56-3.03-1.56-2.09 0-3.8 1.7-3.8 3.8 0 2.1 1.7 3.8 3.8 3.8 1.42 0 2.76-.76 3.49-1.97l2.65-4.41c1-1.67 2.83-2.7 4.77-2.7 2.92 0 5.3 2.38 5.3 5.3s-2.38 5.3-5.3 5.3Z"
			:fill="color"
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
			d="M10.18 9.32a4.474 4.474 0 0 0-3.64-1.87c-2.51 0-4.55 2.04-4.55 4.55s2.04 4.55 4.55 4.55c1.69 0 3.26-.89 4.13-2.34L12 12l1.32-2.21a4.821 4.821 0 0 1 4.13-2.34C19.96 7.45 22 9.49 22 12s-2.04 4.55-4.55 4.55c-1.5 0-2.81-.74-3.64-1.87"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
	</svg>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
	name: 'UnlimitedIcon',
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
