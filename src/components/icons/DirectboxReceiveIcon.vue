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
			d="M18.69 11.53c-.57-.15-1.24-.23-2.04-.23-1.11 0-1.52.27-2.09.7-.03.02-.06.05-.09.08l-.95 1.01c-.8.84-2.24.85-3.04-.01l-.95-1c-.03-.03-.06-.06-.09-.08-.57-.43-.98-.7-2.09-.7-.8 0-1.47.08-2.04.23-2.38.64-2.38 2.53-2.38 4.19v.93c0 2.51 0 5.35 5.35 5.35h7.44c3.55 0 5.35-1.8 5.35-5.35v-.93c0-1.66 0-3.55-2.38-4.19Zm-4.36 6.87H9.67c-.38 0-.69-.31-.69-.7 0-.39.31-.7.69-.7h4.66c.38 0 .69.31.69.7 0 .39-.31.7-.69.7ZM12.668 2.67a.67.67 0 0 0-1.34 0V4h1.35V2.67h-.01Z"
			:fill="color"
		></path>
		<path
			d="M19.21 8.42v1.7c-.04-.02-.09-.03-.13-.04h-.01c-.71-.19-1.5-.28-2.42-.28-1.54 0-2.27.45-2.93.95-.14.1-.24.2-.34.3l-.95 1.01c-.1.1-.26.16-.43.16a.58.58 0 0 1-.43-.17l-.98-1.03c-.1-.11-.22-.2-.25-.22-.72-.55-1.45-1-2.99-1-.92 0-1.71.09-2.43.28-.04.01-.09.02-.13.04v-1.7c0-2.07 0-4.42 4.42-4.42h2.12v3.45l-.65-.65a.676.676 0 0 0-.96.95l1.8 1.8c.01.01.02.01.02.02.06.05.13.1.2.13.09.03.17.05.26.05s.17-.02.26-.05c.08-.03.15-.08.22-.15l1.8-1.8a.676.676 0 0 0-.96-.95l-.65.65V4h2.12c4.42 0 4.42 2.35 4.42 4.42Z"
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
			d="M12 2v6l2-2M12 8l-2-2"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M12 22h4c4 0 5-2.24 5-5v-1c0-2.21 0-4-4-4-1 0-1.28.21-1.8.6l-1.02 1.08a2.999 2.999 0 0 1-4.37 0L8.8 12.6C8.28 12.21 8 12 7 12c-4 0-4 1.79-4 4v1c0 2.76 0 5 5 5M5 12V8c0-2.01 0-3.67 3-3.96M19 12V8c0-2.01 0-3.67-3-3.96"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
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
			d="M14.79 4H9.21C4.79 4 4.79 6.35 4.79 8.42v3.79c0 .22.1.42.27.55.17.13.4.18.61.12.45-.12 1.01-.18 1.68-.18.67 0 .81.08 1.21.38l.91.96a3.48 3.48 0 0 0 5.08 0l.91-.96c.4-.3.54-.38 1.21-.38.67 0 1.23.06 1.68.18.21.06.43.01.61-.12.17-.13.27-.34.27-.55V8.42C19.21 6.35 19.21 4 14.79 4Z"
			:fill="color"
		></path>
		<path
			d="M14.276 6.8a.676.676 0 0 0-.95 0l-.65.65V2.67c0-.37-.31-.67-.68-.67-.37 0-.68.3-.68.67v4.77l-.64-.64a.676.676 0 0 0-.95 0c-.26.26-.26.69 0 .95l1.8 1.8c.01.01.01.01.02.01.06.05.12.1.2.13.08.03.17.05.26.05s.17-.02.26-.05c.08-.03.16-.08.22-.15l1.8-1.8c.25-.25.25-.68-.01-.94ZM18.69 11.53c-.57-.15-1.24-.23-2.04-.23-1.11 0-1.52.27-2.09.7-.03.02-.06.05-.09.08l-.95 1.01c-.8.84-2.24.85-3.04-.01l-.95-1c-.03-.03-.06-.06-.09-.08-.57-.43-.98-.7-2.09-.7-.8 0-1.47.08-2.04.23-2.38.64-2.38 2.53-2.38 4.19v.93c0 2.51 0 5.35 5.35 5.35h7.44c3.55 0 5.35-1.8 5.35-5.35v-.93c0-1.66 0-3.55-2.38-4.19Zm-4.36 6.87H9.67c-.38 0-.69-.31-.69-.7 0-.39.31-.7.69-.7h4.66c.38 0 .69.31.69.7 0 .39-.31.7-.69.7Z"
			:fill="color"
		></path>
		<path
			opacity=".4"
			d="M15.02 17.7c0 .39-.31.7-.69.7H9.67c-.38 0-.69-.31-.69-.7 0-.39.31-.7.69-.7h4.66c.38 0 .69.31.69.7Z"
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
			d="M12 2v6l2-2M12 8l-2-2"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M7 12c-4 0-4 1.79-4 4v1c0 2.76 0 5 5 5h8c4 0 5-2.24 5-5v-1c0-2.21 0-4-4-4-1 0-1.28.21-1.8.6l-1.02 1.08a2.999 2.999 0 0 1-4.37 0L8.8 12.6C8.28 12.21 8 12 7 12ZM5 12V8c0-2.01 0-3.67 3-3.96M19 12V8c0-2.01 0-3.67-3-3.96"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
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
			d="M12 8.75c-.1 0-.19-.02-.29-.06a.74.74 0 0 1-.46-.69V2c0-.41.34-.75.75-.75s.75.34.75.75v4.19l.72-.72c.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06l-2 2c-.14.14-.34.22-.53.22Z"
			:fill="color"
		></path>
		<path
			d="M12.001 8.751c-.19 0-.38-.07-.53-.22l-2-2a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l2 2c.29.29.29.77 0 1.06-.15.15-.34.22-.53.22ZM16 22.75H8c-5.75 0-5.75-3.05-5.75-5.75v-1c0-2.23 0-4.75 4.75-4.75 1.19 0 1.63.29 2.25.75.03.03.07.05.1.09l1.02 1.08c.86.91 2.42.91 3.28 0l1.02-1.08c.03-.03.06-.06.1-.09.62-.47 1.06-.75 2.25-.75 4.75 0 4.75 2.52 4.75 4.75v1c-.02 3.82-1.95 5.75-5.77 5.75Zm-9-10c-3.25 0-3.25 1.02-3.25 3.25v1c0 2.74 0 4.25 4.25 4.25h8c2.98 0 4.25-1.27 4.25-4.25v-1c0-2.23 0-3.25-3.25-3.25-.72 0-.87.09-1.3.41l-.97 1.03A3.73 3.73 0 0 1 12 15.37a3.73 3.73 0 0 1-2.73-1.18l-.97-1.03c-.43-.32-.58-.41-1.3-.41Z"
			:fill="color"
		></path>
		<path
			d="M5 12.75c-.41 0-.75-.34-.75-.75V8c0-1.94 0-4.35 3.68-4.7.41-.04.78.26.82.68.04.41-.26.78-.68.82-2.32.21-2.32 1.15-2.32 3.2v4c0 .41-.34.75-.75.75ZM19.001 12.748c-.41 0-.75-.34-.75-.75v-4c0-2.05 0-2.99-2.32-3.21a.75.75 0 0 1-.67-.82c.04-.41.4-.72.82-.67 3.68.35 3.68 2.76 3.68 4.7v4a.77.77 0 0 1-.76.75Z"
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
		<g
			opacity=".4"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		>
			<path d="M12 2v6l2-2M12 8l-2-2"></path>
		</g>
		<path
			d="M7 12c-4 0-4 1.79-4 4v1c0 2.76 0 5 5 5h8c4 0 5-2.24 5-5v-1c0-2.21 0-4-4-4-1 0-1.28.21-1.8.6l-1.02 1.08a2.999 2.999 0 0 1-4.37 0L8.8 12.6C8.28 12.21 8 12 7 12Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M5 12V8c0-2.01 0-3.67 3-3.96M19 12V8c0-2.01 0-3.67-3-3.96"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
	</svg>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
	name: 'DirectboxReceiveIcon',
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
