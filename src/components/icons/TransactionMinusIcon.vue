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
			d="M15.78 2H8.22C4.44 2 3.5 3.01 3.5 7.04V18.3c0 2.66 1.46 3.29 3.23 1.39l.01-.01c.82-.87 2.07-.8 2.78.15l1.01 1.35c.81 1.07 2.12 1.07 2.93 0l1.01-1.35c.72-.96 1.97-1.03 2.79-.15 1.78 1.9 3.23 1.27 3.23-1.39V7.04C20.5 3.01 19.56 2 15.78 2Zm-1.03 8.75h-5.5c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h5.5c.41 0 .75.34.75.75s-.34.75-.75.75Z"
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
			d="M14.16 10h.59M9.25 10h2.4M3.498 11v7.3c0 2.66 1.46 3.29 3.23 1.39l.01-.01c.82-.87 2.07-.8 2.78.15l1.01 1.35c.81 1.07 2.12 1.07 2.93 0l1.01-1.35c.72-.96 1.97-1.03 2.79-.15 1.78 1.9 3.23 1.27 3.23-1.39V7.04c0-4.03-.94-5.04-4.72-5.04h-7.56c-3.78 0-4.72 1.01-4.72 5.04"
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
			d="M6.728 19.7c.82-.88 2.07-.81 2.79.15l1.01 1.35c.81 1.07 2.12 1.07 2.93 0l1.01-1.35c.72-.96 1.97-1.03 2.79-.15 1.78 1.9 3.23 1.27 3.23-1.39V7.04c0-4.03-.94-5.04-4.72-5.04h-7.56c-3.78 0-4.72 1.01-4.72 5.04V18.3c.01 2.67 1.47 3.29 3.24 1.4Z"
			:fill="color"
		></path>
		<path
			d="M14.75 10.75h-5.5c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h5.5c.41 0 .75.34.75.75s-.34.75-.75.75Z"
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
			d="M6.728 19.7c.82-.88 2.07-.81 2.79.15l1.01 1.35c.81 1.07 2.12 1.07 2.93 0l1.01-1.35c.72-.96 1.97-1.03 2.79-.15 1.78 1.9 3.23 1.27 3.23-1.39V7.04c0-4.03-.94-5.04-4.72-5.04h-7.56c-3.78 0-4.72 1.01-4.72 5.04V18.3c.01 2.67 1.47 3.29 3.24 1.4ZM9.25 10h5.5"
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
			d="M12 22.75c-.78 0-1.54-.4-2.06-1.1L8.93 20.3c-.21-.28-.49-.44-.79-.46-.3-.01-.6.12-.84.37l-.55-.51.55.51c-1.44 1.54-2.55 1.42-3.08 1.21-.54-.21-1.45-.9-1.45-3.12V7.04c0-4.44 1.28-5.79 5.47-5.79h7.56c4.19 0 5.47 1.35 5.47 5.79V18.3c0 2.21-.91 2.9-1.45 3.12-.53.21-1.63.33-3.08-1.21-.24-.26-.54-.39-.85-.37-.3.02-.59.18-.8.46l-1.01 1.35c-.54.7-1.3 1.1-2.08 1.1Zm-3.92-4.42h.13c.74.04 1.44.43 1.91 1.06l1.01 1.35c.49.65 1.24.65 1.73 0l1.01-1.35c.48-.63 1.17-1.02 1.92-1.06.75-.04 1.48.27 2.02.85.76.81 1.25.91 1.43.84.24-.1.5-.68.5-1.72V7.04c0-3.61-.63-4.29-3.97-4.29H8.21c-3.34 0-3.97.68-3.97 4.29V18.3c0 1.05.26 1.63.5 1.72.17.07.67-.03 1.43-.84.55-.55 1.22-.85 1.91-.85Z"
			:fill="color"
		></path>
		<path
			d="M14.75 10.75h-5.5c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h5.5c.41 0 .75.34.75.75s-.34.75-.75.75Z"
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
			d="M6.728 19.7c.82-.88 2.07-.81 2.79.15l1.01 1.35c.81 1.07 2.12 1.07 2.93 0l1.01-1.35c.72-.96 1.97-1.03 2.79-.15 1.78 1.9 3.23 1.27 3.23-1.39V7.04c0-4.03-.94-5.04-4.72-5.04h-7.56c-3.78 0-4.72 1.01-4.72 5.04V18.3c.01 2.67 1.47 3.29 3.24 1.4Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M9.25 10h5.5"
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
	name: 'TransactionMinusIcon',
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
