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
			d="M20.619 8.7c-1.04-4.63-5.08-6.7-8.62-6.7h-.01c-3.53 0-7.56 2.07-8.61 6.69-1.18 5.16 1.98 9.53 4.84 12.29a5.436 5.436 0 0 0 3.78 1.53c1.36 0 2.72-.51 3.77-1.53 2.86-2.76 6.02-7.12 4.85-12.28Zm-5.87 3.05h-2v2c0 .41-.34.75-.75.75s-.75-.34-.75-.75v-2h-2c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h2v-2c0-.41.34-.75.75-.75s.75.34.75.75v2h2c.41 0 .75.34.75.75s-.34.75-.75.75Z"
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
			d="M9.25 11h5.5M12 13.75v-5.5"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
		></path>
		<path
			d="M5.98 4.3c4.37-4.11 12.84-2.7 14.4 4.21 1.15 5.08-2.01 9.38-4.78 12.04a5.193 5.193 0 0 1-7.21 0C5.63 17.88 2.46 13.58 3.62 8.5"
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
			d="M20.619 8.7c-1.04-4.63-5.08-6.7-8.62-6.7h-.01c-3.53 0-7.56 2.07-8.61 6.69-1.18 5.16 1.98 9.53 4.84 12.29a5.436 5.436 0 0 0 3.78 1.53c1.36 0 2.72-.51 3.77-1.53 2.86-2.76 6.02-7.12 4.85-12.28Z"
			:fill="color"
		></path>
		<path
			d="M14.75 10.25h-2v-2c0-.41-.34-.75-.75-.75s-.75.34-.75.75v2h-2c-.41 0-.75.34-.75.75s.34.75.75.75h2v2c0 .41.34.75.75.75s.75-.34.75-.75v-2h2c.41 0 .75-.34.75-.75s-.34-.75-.75-.75Z"
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
			d="M9.25 11h5.5M12 13.75v-5.5"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
		></path>
		<path
			d="M3.62 8.49c1.97-8.66 14.8-8.65 16.76.01 1.15 5.08-2.01 9.38-4.78 12.04a5.193 5.193 0 0 1-7.21 0c-2.76-2.66-5.92-6.97-4.77-12.05Z"
			:stroke="color"
			:stroke-width="strokeWidth"
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
			d="M14.75 11.75h-5.5c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h5.5c.41 0 .75.34.75.75s-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M12 14.5c-.41 0-.75-.34-.75-.75v-5.5c0-.41.34-.75.75-.75s.75.34.75.75v5.5c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M12.002 22.76a5.97 5.97 0 0 1-4.13-1.67c-2.95-2.84-6.21-7.37-4.98-12.76 1.11-4.89 5.38-7.08 9.11-7.08h.01c3.73 0 8 2.19 9.11 7.09 1.22 5.39-2.04 9.91-4.99 12.75a5.97 5.97 0 0 1-4.13 1.67Zm0-20.01c-2.91 0-6.65 1.55-7.64 5.91-1.08 4.71 1.88 8.77 4.56 11.34a4.425 4.425 0 0 0 6.17 0c2.67-2.57 5.63-6.63 4.57-11.34-1-4.36-4.75-5.91-7.66-5.91Z"
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
		<g opacity=".4">
			<path
				:stroke="color"
				stroke-linecap="round"
				:stroke-width="strokeWidth"
				d="M9.25 11h5.5M12 13.75v-5.5"
			></path>
		</g>
		<path
			:stroke="color"
			:stroke-width="strokeWidth"
			d="M3.62 8.49c1.97-8.66 14.8-8.65 16.76.01 1.15 5.08-2.01 9.38-4.78 12.04a5.193 5.193 0 01-7.21 0c-2.76-2.66-5.92-6.97-4.77-12.05z"
		></path>
	</svg>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
	name: 'LocationAddIcon',
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
