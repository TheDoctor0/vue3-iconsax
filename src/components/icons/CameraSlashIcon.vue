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
			d="M21.769 2.229c-.3-.3-.79-.3-1.09 0l-18.45 18.46c-.3.3-.3.79 0 1.09a.758.758 0 0 0 1.08-.01l18.46-18.46c.31-.3.31-.78 0-1.08Z"
			:fill="color"
		></path>
		<path
			d="m16.55 5.11-.72-1.45C15.37 2.75 14.17 2 13.15 2h-2.29c-1.03 0-2.23.75-2.69 1.66l-.72 1.45C7.17 5.65 6.61 6 6 6 3.83 6 2.11 7.83 2.25 9.99l.52 8.26c.05.85.26 1.64.71 2.27L18 6c-.61 0-1.17-.35-1.45-.89ZM9.5 10.75h-3c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h3c.41 0 .75.34.75.75s-.34.75-.75.75ZM21.75 9.988l-.52 8.26c-.13 2.06-1.23 3.75-3.99 3.75H7.41c-.89 0-1.34-1.08-.71-1.71l2.47-2.47c.31-.31.79-.35 1.18-.13.69.39 1.52.54 2.4.35 1.27-.27 2.3-1.31 2.55-2.59.17-.86.02-1.67-.36-2.34-.22-.39-.19-.88.13-1.19l4.5-4.5a.965.965 0 0 1 1.45.11c.52.68.79 1.54.73 2.46Z"
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
			d="M6 10h3M6.762 22.002h10.48c2.76 0 3.86-1.69 3.99-3.75l.52-8.26c.06-.93-.23-1.8-.74-2.48M2.77 18.25c.05.82.26 1.59.67 2.21M18 6c-.61 0-1.17-.35-1.45-.89l-.72-1.45C15.37 2.75 14.17 2 13.15 2h-2.29c-1.03 0-2.23.75-2.69 1.66l-.72 1.45C7.17 5.65 6.61 6 6 6 3.83 6 2.11 7.83 2.25 9.99l.25 4.03"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M10 17.31c.55.43 1.25.69 2 .69 1.79 0 3.25-1.46 3.25-3.25 0-.64-.18-1.23-.5-1.73M22 2 2 22"
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
			d="M21.769 2.229c-.3-.3-.79-.3-1.09 0l-18.45 18.46c-.3.3-.3.79 0 1.09a.758.758 0 0 0 1.08-.01l18.46-18.46c.31-.3.31-.78 0-1.08Z"
			:fill="color"
		></path>
		<path
			opacity=".4"
			d="m21.749 9.99-.52 8.26c-.13 2.06-1.23 3.75-3.99 3.75H6.759c-.59 0-1.1-.08-1.54-.22l15.03-15.03c.98.73 1.59 1.92 1.5 3.24ZM18 6 3.48 20.52c-.45-.63-.66-1.42-.71-2.27l-.52-8.26A3.753 3.753 0 0 1 6 6c.61 0 1.17-.35 1.45-.89l.72-1.45C8.63 2.75 9.83 2 10.86 2h2.29c1.02 0 2.22.75 2.68 1.66l.72 1.45c.28.54.84.89 1.45.89Z"
			:fill="color"
		></path>
		<path
			d="M9.5 10.75h-3c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h3c.41 0 .75.34.75.75s-.34.75-.75.75ZM12.569 11.429l-3.89 3.89a3.372 3.372 0 0 1 3.89-3.89ZM15.38 14.75A3.38 3.38 0 0 1 12 18.12c-.87 0-1.66-.33-2.25-.87l4.75-4.75c.55.59.88 1.38.88 2.25Z"
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
			d="M6 10h3M6.76 22h10.48c2.76 0 3.86-1.69 3.99-3.75l.52-8.26c.06-.93-.23-1.8-.74-2.48M18 6c-.61 0-1.17-.35-1.45-.89l-.72-1.45C15.37 2.75 14.17 2 13.15 2h-2.29c-1.03 0-2.23.75-2.69 1.66l-.72 1.45C7.17 5.65 6.61 6 6 6 3.83 6 2.11 7.83 2.25 9.99l.52 8.26c.05.82.26 1.59.67 2.21"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M10 17.31c.55.43 1.25.69 2 .69 1.79 0 3.25-1.46 3.25-3.25 0-.64-.18-1.23-.5-1.73M22 2 2 22"
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
			d="M9 10.75H6c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h3c.41 0 .75.34.75.75s-.34.75-.75.75ZM17.242 22.748H6.762c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h10.48c2.02 0 3.11-1.03 3.24-3.05l.52-8.26a2.94 2.94 0 0 0-.59-1.98.75.75 0 0 1 1.2-.9c.64.86.96 1.91.89 2.98l-.52 8.26c-.18 2.83-1.91 4.45-4.74 4.45Z"
			:fill="color"
		></path>
		<path
			d="M3.442 21.21c-.24 0-.48-.12-.63-.34-.46-.7-.73-1.57-.79-2.58l-.52-8.25a4.44 4.44 0 0 1 1.21-3.36c.85-.91 2.05-1.43 3.29-1.43.32 0 .63-.19.78-.49l.72-1.43c.59-1.17 2.07-2.08 3.36-2.08h2.29c1.29 0 2.76.91 3.35 2.07l.72 1.46c.15.28.45.47.78.47.41 0 .75.34.75.75s-.34.75-.75.75c-.89 0-1.7-.5-2.12-1.29L15.152 4c-.33-.66-1.27-1.24-2.01-1.24h-2.29c-.74 0-1.68.58-2.02 1.25l-.71 1.43c-.42.81-1.23 1.31-2.12 1.31-.84 0-1.62.34-2.2.95-.57.61-.86 1.41-.8 2.24l.52 8.26c.04.73.23 1.37.55 1.84a.753.753 0 0 1-.63 1.17ZM12.002 18.748c-.89 0-1.76-.3-2.46-.85a.75.75 0 0 1 .92-1.18 2.5 2.5 0 0 0 4.04-1.97c0-.48-.13-.94-.38-1.33a.758.758 0 0 1 .23-1.04c.35-.22.81-.12 1.04.23.4.63.62 1.37.62 2.13a4.016 4.016 0 0 1-4.01 4.01Z"
			:fill="color"
		></path>
		<path
			d="M2.001 22.751c-.19 0-.38-.07-.53-.22a.754.754 0 0 1 0-1.06l20-20c.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06l-20 20c-.15.15-.34.22-.53.22Z"
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
			d="M6 10h3M6.762 22.002h10.48c2.76 0 3.86-1.69 3.99-3.75l.52-8.26c.06-.93-.23-1.8-.74-2.48"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M18 6c-.61 0-1.17-.35-1.45-.89l-.72-1.45C15.37 2.75 14.17 2 13.15 2h-2.29c-1.03 0-2.23.75-2.69 1.66l-.72 1.45C7.17 5.65 6.61 6 6 6 3.83 6 2.11 7.83 2.25 9.99l.52 8.26c.05.82.26 1.59.67 2.21"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M10 17.31c.55.43 1.25.69 2 .69 1.79 0 3.25-1.46 3.25-3.25 0-.64-.18-1.23-.5-1.73"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 2 2 22"
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
	name: 'CameraSlashIcon',
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
