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
			d="M12.75 14.52h.23c.33 0 .61-.3.61-.67 0-.47-.11-.53-.43-.64l-.41-.14v1.45z"
		></path>
		<path
			:fill="color"
			d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zM7.58 16.42c.29.29.29.77 0 1.06-.15.15-.34.22-.53.22s-.38-.07-.53-.22A7.709 7.709 0 014.25 12c0-2.07.81-4.02 2.27-5.48.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06A6.21 6.21 0 005.75 12c0 1.67.65 3.24 1.83 4.42zm6.07-4.64c.96.34 1.43 1.01 1.43 2.06 0 1.2-.94 2.17-2.11 2.17h-.23v.18c0 .41-.34.75-.75.75s-.75-.34-.75-.75v-.18h-.03c-1.27 0-2.31-1.07-2.31-2.38 0-.41.34-.75.75-.75s.75.34.75.75c0 .49.36.88.81.88h.03v-1.98l-.9-.32c-.96-.34-1.43-1.01-1.43-2.06 0-1.2.94-2.17 2.11-2.17h.23V7.8c0-.41.34-.75.75-.75s.75.34.75.75v.18h.03c1.27 0 2.31 1.07 2.31 2.38 0 .41-.34.75-.75.75s-.75-.34-.75-.75c0-.49-.36-.88-.81-.88h-.03v1.98l.9.32zm3.83 5.7c-.15.15-.34.22-.53.22s-.38-.07-.53-.22a.754.754 0 010-1.06A6.21 6.21 0 0018.25 12c0-1.67-.65-3.24-1.83-4.42a.754.754 0 010-1.06c.29-.29.77-.29 1.06 0A7.709 7.709 0 0119.75 12c0 2.07-.81 4.02-2.27 5.48z"
		></path>
		<path
			:fill="color"
			d="M10.42 10.16c0 .47.11.53.43.64l.41.14V9.48h-.23c-.34 0-.61.31-.61.68z"
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
			d="M16.95 16.95a7.007 7.007 0 0 0 0-9.9M7.05 7.05a7.007 7.007 0 0 0 0 9.9"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M9.67 13.628c0 .9.7 1.63 1.56 1.63h1.76c.75 0 1.36-.64 1.36-1.42 0-.85-.37-1.16-.93-1.35l-2.81-.98c-.55-.19-.93-.5-.93-1.35 0-.79.61-1.42 1.36-1.42h1.76c.86 0 1.56.73 1.56 1.63M12 7.8v8.4"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M4 6c-1.25 1.67-2 3.75-2 6 0 5.52 4.48 10 10 10s10-4.48 10-10S17.52 2 12 2c-1.43 0-2.8.3-4.03.85"
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
			d="M12 22c5.523 0 10-4.477 10-10S17.523 2 12 2 2 6.477 2 12s4.477 10 10 10Z"
			:fill="color"
		></path>
		<path
			d="M16.95 17.698c-.19 0-.38-.07-.53-.22a.754.754 0 0 1 0-1.06 6.21 6.21 0 0 0 1.83-4.42c0-1.67-.65-3.24-1.83-4.42a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0a7.709 7.709 0 0 1 2.27 5.48c0 2.07-.81 4.02-2.27 5.48-.15.15-.34.22-.53.22ZM7.05 17.698c-.19 0-.38-.07-.53-.22a7.709 7.709 0 0 1-2.27-5.48c0-2.07.81-4.02 2.27-5.48.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06a6.21 6.21 0 0 0-1.83 4.42c0 1.67.65 3.24 1.83 4.42.29.29.29.77 0 1.06-.15.15-.34.22-.53.22ZM13.65 11.78l-.9-.32V9.48h.03c.44 0 .81.4.81.88 0 .41.34.75.75.75s.75-.34.75-.75c0-1.31-1.03-2.38-2.31-2.38h-.03V7.8c0-.41-.34-.75-.75-.75s-.75.34-.75.75v.18h-.23c-1.16 0-2.11.98-2.11 2.17 0 1.05.47 1.72 1.43 2.06l.9.32v1.98h-.03c-.44 0-.81-.4-.81-.88 0-.41-.34-.75-.75-.75s-.75.34-.75.75c0 1.31 1.03 2.38 2.31 2.38h.03v.18c0 .41.34.75.75.75s.75-.34.75-.75v-.18h.23c1.16 0 2.11-.98 2.11-2.17 0-1.05-.46-1.72-1.43-2.06Zm-2.81-.98c-.32-.11-.43-.17-.43-.64 0-.37.27-.67.61-.67h.23v1.46l-.41-.15Zm2.14 3.72h-.23v-1.46l.41.14c.32.11.43.17.43.64-.01.37-.28.68-.61.68Z"
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
			d="M16.9 16.9c2.7-2.7 2.7-7.2 0-9.9M7.1 7.1c-2.7 2.7-2.7 7.2 0 9.9"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M9.7 13.6c0 .9.7 1.6 1.6 1.6H13c.7 0 1.4-.6 1.4-1.4 0-.9-.4-1.2-.9-1.4l-2.8-1c-.7-.1-1-.4-1-1.2 0-.8.6-1.4 1.4-1.4h1.8c.9 0 1.6.7 1.6 1.6M12 7.8v8.4"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M12 22c5.523 0 10-4.477 10-10S17.523 2 12 2 2 6.477 2 12s4.477 10 10 10Z"
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
			d="M16.95 17.698c-.19 0-.38-.07-.53-.22a.754.754 0 0 1 0-1.06 6.21 6.21 0 0 0 1.83-4.42c0-1.67-.65-3.24-1.83-4.42a.755.755 0 0 1 0-1.06c.29-.29.77-.29 1.06 0a7.709 7.709 0 0 1 2.27 5.48c0 2.07-.81 4.02-2.27 5.48-.15.15-.34.22-.53.22ZM7.05 17.698c-.19 0-.38-.07-.53-.22a7.709 7.709 0 0 1-2.27-5.48c0-2.07.81-4.02 2.27-5.48.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06a6.21 6.21 0 0 0-1.83 4.42c0 1.67.65 3.24 1.83 4.42.29.29.29.77 0 1.06-.15.15-.34.22-.53.22ZM12.98 16.02h-1.76c-1.27 0-2.31-1.07-2.31-2.38 0-.41.34-.75.75-.75s.75.34.75.75c0 .49.36.88.81.88h1.76c.33 0 .61-.3.61-.67 0-.47-.11-.53-.43-.64l-2.81-.98c-.96-.34-1.43-1.01-1.43-2.06 0-1.2.94-2.17 2.11-2.17h1.76c1.27 0 2.31 1.07 2.31 2.38 0 .41-.34.75-.75.75s-.75-.34-.75-.75c0-.49-.36-.88-.81-.88h-1.76c-.33 0-.61.3-.61.67 0 .47.11.53.43.64l2.81.98c.96.34 1.43 1.01 1.43 2.06-.01 1.19-.95 2.17-2.11 2.17Z"
			:fill="color"
		></path>
		<path
			d="M12 16.95c-.41 0-.75-.34-.75-.75V7.8c0-.41.34-.75.75-.75s.75.34.75.75v8.4c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M12 22.75C6.07 22.75 1.25 17.93 1.25 12S6.07 1.25 12 1.25 22.75 6.07 22.75 12 17.93 22.75 12 22.75Zm0-20C6.9 2.75 2.75 6.9 2.75 12S6.9 21.25 12 21.25s9.25-4.15 9.25-9.25S17.1 2.75 12 2.75Z"
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
			d="M16.95 16.95a7.007 7.007 0 0 0 0-9.9M7.05 7.05a7.007 7.007 0 0 0 0 9.9"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<g
			opacity=".4"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		>
			<path
				d="M9.67 13.632c0 .9.7 1.63 1.56 1.63h1.76c.75 0 1.36-.64 1.36-1.42 0-.85-.37-1.16-.93-1.35l-2.81-.98c-.55-.19-.93-.5-.93-1.35 0-.79.61-1.42 1.36-1.42h1.76c.86 0 1.56.73 1.56 1.63M12 7.8v8.4"
			></path>
		</g>
		<path
			d="M12 22c5.523 0 10-4.477 10-10S17.523 2 12 2 2 6.477 2 12s4.477 10 10 10Z"
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
	name: 'UsdCoinIcon',
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
