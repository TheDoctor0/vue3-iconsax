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
			d="M12 14c-5.01 0-9.09 3.36-9.09 7.5 0 .28.22.5.5.5h17.18c.28 0 .5-.22.5-.5 0-4.14-4.08-7.5-9.09-7.5ZM16.85 5.798c-.12-.49-.32-.97-.6-1.41-.19-.32-.44-.64-.71-.92a4.96 4.96 0 0 0-3.27-1.45c-1.36-.09-2.75.41-3.8 1.45A4.96 4.96 0 0 0 7 7.078c.01 1.25.51 2.5 1.46 3.46.66.66 1.47 1.1 2.34 1.3.47.12.97.18 1.47.14 1.19-.05 2.35-.52 3.26-1.44a4.984 4.984 0 0 0 1.32-4.74ZM14 8.998c-.36.36-.96.36-1.32 0l-.69-.69-.66.66c-.36.36-.96.36-1.32 0a.933.933 0 0 1-.01-1.32l.66-.66-.64-.62a.966.966 0 0 1 0-1.34c.37-.36.96-.36 1.34 0l.62.64.67-.67c.36-.36.95-.36 1.32 0 .36.36.36.96 0 1.32l-.66.66.69.7c.36.36.36.96 0 1.32Z"
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
			d="M15.02 3.01A4.944 4.944 0 0 0 12 2C9.24 2 7 4.24 7 7s2.24 5 5 5 5-2.24 5-5M3.41 22c0-3.87 3.85-7 8.59-7 .96 0 1.89.13 2.76.37"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 18c0 .32-.04.63-.12.93-.09.4-.25.79-.46 1.13A3.97 3.97 0 0 1 18 22a3.92 3.92 0 0 1-2.66-1.03c-.3-.26-.56-.57-.76-.91A3.92 3.92 0 0 1 14 18a3.995 3.995 0 0 1 4-4c1.18 0 2.25.51 2.97 1.33.64.71 1.03 1.65 1.03 2.67ZM19.032 16.941l-2.11 2.11M16.941 16.96l2.12 2.11"
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
			d="M21.09 21.5c0 .28-.22.5-.5.5H3.41c-.28 0-.5-.22-.5-.5 0-4.14 4.08-7.5 9.09-7.5 1.03 0 2.03.14 2.95.41-.59.7-.95 1.61-.95 2.59 0 .75.21 1.46.58 2.06.2.34.46.65.76.91.7.64 1.63 1.03 2.66 1.03 1.12 0 2.13-.46 2.85-1.2.16.54.24 1.11.24 1.7Z"
			:fill="color"
		></path>
		<path
			d="M21.88 16.042c-.1-.39-.26-.78-.48-1.13-.15-.26-.35-.51-.57-.74a3.988 3.988 0 0 0-2.62-1.16c-1.09-.07-2.2.33-3.04 1.16a4.007 4.007 0 0 0 0 5.66c.53.53 1.18.88 1.87 1.04.38.1.78.14 1.18.11.95-.04 1.88-.42 2.61-1.15a3.98 3.98 0 0 0 1.05-3.79Zm-2.28 2.56c-.29.29-.77.29-1.06 0l-.55-.55-.53.53c-.29.29-.77.29-1.06 0a.754.754 0 0 1 0-1.06l.53-.53-.51-.5a.767.767 0 0 1 0-1.07c.3-.29.77-.29 1.07 0l.5.51.53-.53c.29-.29.76-.29 1.06 0 .29.29.29.77 0 1.06l-.53.53.55.55c.29.29.29.77 0 1.06ZM12 12a5 5 0 1 0 0-10 5 5 0 0 0 0 10Z"
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
			d="M12 12a5 5 0 1 0 0-10 5 5 0 0 0 0 10ZM3.41 22c0-3.87 3.85-7 8.59-7 .96 0 1.89.13 2.76.37"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 18c0 .32-.04.63-.12.93-.09.4-.25.79-.46 1.13A3.97 3.97 0 0 1 18 22a3.92 3.92 0 0 1-2.66-1.03c-.3-.26-.56-.57-.76-.91A3.92 3.92 0 0 1 14 18a3.995 3.995 0 0 1 4-4c1.18 0 2.25.51 2.97 1.33.64.71 1.03 1.65 1.03 2.67ZM19.03 16.94l-2.11 2.11M16.94 16.96l2.12 2.11"
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
			d="M12 12.75c-3.17 0-5.75-2.58-5.75-5.75S8.83 1.25 12 1.25 17.75 3.83 17.75 7s-2.58 5.75-5.75 5.75Zm0-10A4.26 4.26 0 0 0 7.75 7 4.26 4.26 0 0 0 12 11.25 4.26 4.26 0 0 0 16.25 7 4.26 4.26 0 0 0 12 2.75ZM3.41 22.75c-.41 0-.75-.34-.75-.75 0-4.27 4.19-7.75 9.34-7.75 1.01 0 2 .13 2.96.4.4.11.63.52.52.92-.11.4-.52.63-.92.52-.82-.23-1.68-.34-2.56-.34-4.32 0-7.84 2.8-7.84 6.25 0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M18 22.75a4.7 4.7 0 0 1-3.17-1.23c-.35-.3-.66-.67-.9-1.08-.44-.72-.68-1.57-.68-2.44 0-1.25.48-2.42 1.34-3.31.9-.93 2.11-1.44 3.41-1.44 1.36 0 2.65.58 3.53 1.58A4.74 4.74 0 0 1 22.75 18c0 .38-.05.76-.15 1.12-.1.45-.29.92-.55 1.33-.83 1.42-2.39 2.3-4.05 2.3Zm0-8a3.241 3.241 0 0 0-2.78 4.92c.16.28.37.53.61.74.6.55 1.37.85 2.17.85 1.13 0 2.2-.6 2.78-1.57.17-.28.3-.6.37-.91.07-.26.1-.51.1-.77 0-.8-.3-1.57-.84-2.17-.6-.7-1.48-1.09-2.41-1.09Z"
			:fill="color"
		></path>
		<path
			d="M16.92 19.799c-.19 0-.38-.07-.53-.22a.754.754 0 0 1 0-1.06l2.11-2.11c.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06l-2.11 2.11c-.15.15-.34.22-.53.22Z"
			:fill="color"
		></path>
		<path
			d="M19.06 19.819c-.19 0-.38-.07-.53-.22l-2.11-2.11a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l2.11 2.11c.29.29.29.77 0 1.06-.15.15-.34.22-.53.22Z"
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
			d="M12 12a5 5 0 1 0 0-10 5 5 0 0 0 0 10Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M3.41 22c0-3.87 3.85-7 8.59-7 .96 0 1.89.13 2.76.37"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 18c0 .32-.04.63-.12.93-.09.4-.25.79-.46 1.13A3.97 3.97 0 0 1 18 22a3.92 3.92 0 0 1-2.66-1.03c-.3-.26-.56-.57-.76-.91A3.92 3.92 0 0 1 14 18a3.995 3.995 0 0 1 4-4c1.18 0 2.25.51 2.97 1.33.64.71 1.03 1.65 1.03 2.67ZM19.032 16.941l-2.11 2.11M16.941 16.96l2.12 2.11"
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
	name: 'UserRemoveIcon',
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
