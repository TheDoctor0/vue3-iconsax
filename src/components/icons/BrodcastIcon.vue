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
			d="M12.001 14.381a2.38 2.38 0 1 0 0-4.76 2.38 2.38 0 0 0 0 4.76ZM20 18.75a.75.75 0 0 1-.6-1.2A9.17 9.17 0 0 0 21.25 12c0-2.02-.64-3.94-1.85-5.55a.75.75 0 0 1 1.2-.9c1.41 1.87 2.15 4.1 2.15 6.45 0 2.35-.74 4.58-2.15 6.45-.15.2-.37.3-.6.3ZM4 18.75c-.23 0-.45-.1-.6-.3-1.41-1.87-2.15-4.1-2.15-6.45 0-2.35.74-4.58 2.15-6.45a.75.75 0 0 1 1.2.9A9.17 9.17 0 0 0 2.75 12c0 2.02.64 3.94 1.85 5.55a.75.75 0 0 1-.6 1.2ZM16.801 16.349a.75.75 0 0 1-.6-1.2c.69-.91 1.05-2 1.05-3.15s-.36-2.24-1.05-3.15a.75.75 0 0 1 1.2-.9 6.73 6.73 0 0 1 1.35 4.05c0 1.47-.47 2.88-1.35 4.05-.15.2-.37.3-.6.3ZM7.2 16.349c-.23 0-.45-.1-.6-.3a6.709 6.709 0 0 1-1.35-4.05c0-1.47.47-2.88 1.35-4.05a.75.75 0 0 1 1.2.9c-.69.91-1.05 2-1.05 3.15s.36 2.24 1.05 3.15a.75.75 0 0 1-.6 1.2Z"
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
			d="M12 10c-1.1 0-2 .9-2 2s.9 2 2 2 2-.9 2-2M20 18c1.26-1.67 2-3.75 2-6s-.74-4.33-2-6M4 17.999a9.926 9.926 0 0 1-1.98-6.62M4 6c-.38.51-.72 1.06-1 1.64M16.8 15.598c.75-1 1.2-2.25 1.2-3.6s-.45-2.6-1.2-3.6M7.2 8.398c-.75 1-1.2 2.25-1.2 3.6s.45 2.6 1.2 3.6"
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
			d="M12.001 14.381a2.38 2.38 0 1 0 0-4.76 2.38 2.38 0 0 0 0 4.76Z"
			:fill="color"
		></path>
		<path
			opacity=".4"
			d="M20 18.75a.75.75 0 0 1-.6-1.2A9.17 9.17 0 0 0 21.25 12c0-2.02-.64-3.94-1.85-5.55a.75.75 0 0 1 1.2-.9c1.41 1.87 2.15 4.1 2.15 6.45 0 2.35-.74 4.58-2.15 6.45-.15.2-.37.3-.6.3ZM4 18.75c-.23 0-.45-.1-.6-.3-1.41-1.87-2.15-4.1-2.15-6.45 0-2.35.74-4.58 2.15-6.45a.75.75 0 0 1 1.2.9A9.17 9.17 0 0 0 2.75 12c0 2.02.64 3.94 1.85 5.55a.75.75 0 0 1-.6 1.2ZM16.801 16.349a.75.75 0 0 1-.6-1.2c.69-.91 1.05-2 1.05-3.15s-.36-2.24-1.05-3.15a.75.75 0 0 1 1.2-.9 6.73 6.73 0 0 1 1.35 4.05c0 1.47-.47 2.88-1.35 4.05-.15.2-.37.3-.6.3ZM7.2 16.349c-.23 0-.45-.1-.6-.3a6.73 6.73 0 0 1-1.35-4.05c0-1.47.47-2.88 1.35-4.05a.75.75 0 0 1 1.2.9c-.69.91-1.05 2-1.05 3.15s.36 2.24 1.05 3.15a.75.75 0 0 1-.6 1.2Z"
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
			d="M12 14a2 2 0 1 0 0-4 2 2 0 0 0 0 4ZM20 18c1.26-1.67 2-3.75 2-6s-.74-4.33-2-6M4 6c-1.26 1.67-2 3.75-2 6s.74 4.33 2 6M16.8 15.6c.75-1 1.2-2.25 1.2-3.6s-.45-2.6-1.2-3.6M7.2 8.4C6.45 9.4 6 10.65 6 12s.45 2.6 1.2 3.6"
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
			d="M12 14.75c-1.52 0-2.75-1.23-2.75-2.75S10.48 9.25 12 9.25s2.75 1.23 2.75 2.75-1.23 2.75-2.75 2.75Zm0-4a1.25 1.25 0 1 0 0 2.5 1.25 1.25 0 0 0 0-2.5ZM20 18.75a.75.75 0 0 1-.6-1.2A9.17 9.17 0 0 0 21.25 12c0-2.02-.64-3.94-1.85-5.55a.75.75 0 0 1 1.2-.9c1.41 1.87 2.15 4.1 2.15 6.45 0 2.35-.74 4.58-2.15 6.45-.15.2-.37.3-.6.3ZM4 18.75c-.23 0-.45-.1-.6-.3-1.41-1.87-2.15-4.1-2.15-6.45 0-2.35.74-4.58 2.15-6.45a.75.75 0 0 1 1.2.9A9.17 9.17 0 0 0 2.75 12c0 2.02.64 3.94 1.85 5.55a.75.75 0 0 1-.6 1.2ZM16.801 16.349a.75.75 0 0 1-.6-1.2c.69-.91 1.05-2 1.05-3.15s-.36-2.24-1.05-3.15a.75.75 0 0 1 1.2-.9 6.73 6.73 0 0 1 1.35 4.05c0 1.47-.47 2.88-1.35 4.05-.15.2-.37.3-.6.3ZM7.2 16.349c-.23 0-.45-.1-.6-.3a6.73 6.73 0 0 1-1.35-4.05c0-1.47.47-2.88 1.35-4.05a.75.75 0 0 1 1.2.9c-.69.91-1.05 2-1.05 3.15s.36 2.24 1.05 3.15a.75.75 0 0 1-.6 1.2Z"
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
			opacity=".4"
			d="M12 14a2 2 0 1 0 0-4 2 2 0 0 0 0 4Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M20 18c1.26-1.67 2-3.75 2-6s-.74-4.33-2-6M4 6c-1.26 1.67-2 3.75-2 6s.74 4.33 2 6"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M16.8 15.598c.75-1 1.2-2.25 1.2-3.6s-.45-2.6-1.2-3.6M7.2 8.398c-.75 1-1.2 2.25-1.2 3.6s.45 2.6 1.2 3.6"
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
	name: 'BrodcastIcon',
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
