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
			d="M8.93 2H5.02C3 2 2 3 2 5.02v3.92C2 11 3 12 5.02 11.95h3.92C11 12 12 11 11.95 8.93V5.02C12 3 11 2 8.93 2Zm.08 7.76c-.68 0-1.34-.26-1.89-.72a3.7 3.7 0 0 1-2.18.72c-.41 0-.75-.34-.75-.75s.34-.75.75-.75c1.02 0 1.87-.7 2.18-1.66H4.94c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h1.29c.04-.38.35-.68.74-.68s.7.3.74.68H9a.749.749 0 1 1 0 1.5h-.33c-.09.48-.28.93-.53 1.34.27.2.56.32.87.32.41 0 .75.34.75.75s-.34.75-.75.75ZM9 22.75c-4.27 0-7.75-3.48-7.75-7.75 0-.41.34-.75.75-.75s.75.34.75.75c0 2.96 2.06 5.44 4.83 6.09l-.27-.45a.751.751 0 1 1 1.29-.77l1.05 1.75c.14.23.14.52.01.75-.14.23-.39.38-.66.38ZM21.998 9.75c-.41 0-.75-.34-.75-.75 0-2.96-2.06-5.44-4.83-6.09l.27.45a.751.751 0 1 1-1.29.77l-1.05-1.75a.745.745 0 0 1-.01-.75c.14-.23.39-.38.66-.38 4.27 0 7.75 3.48 7.75 7.75 0 .41-.34.75-.75.75ZM16.92 11.852a5.08 5.08 0 1 0 .001 10.161 5.08 5.08 0 0 0-.001-10.161Zm2.48 7.49c-.37.18-.82.04-1.01-.34l-.17-.34h-2.59l-.17.34c-.13.26-.4.41-.67.41-.11 0-.23-.03-.33-.08a.763.763 0 0 1-.34-1.01l2.14-4.27a.76.76 0 0 1 .67-.41c.28 0 .54.16.67.42l2.14 4.27c.18.37.03.82-.34 1.01Z"
			:fill="color"
		></path>
		<path
			d="M16.379 17.16h1.09l-.55-1.09-.54 1.09Z"
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
			d="m19.061 18.668-2.14-4.27-2.14 4.27M15.172 17.91h3.52"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M19.922 21.02c-.84.61-1.87.98-2.99.98a5.08 5.08 0 1 1 5.08-5.08M11.95 8.928c.05 2.07-.95 3.07-3.02 3.02H5.01C3 11.998 2 10.998 2 8.928v-3.92c0-2.02 1-3.02 3.02-3.02h3.92c2.07 0 3.07 1 3.02 3.02M9.013 5.852h-4.06M6.973 5.172v.68"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M7.991 5.844c0 1.75-1.37 3.17-3.05 3.17"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M9.01 9.01c-.73 0-1.39-.39-1.85-1.01M2 15c0 3.87 3.13 7 7 7l-1.05-1.75M22 9c0-3.87-3.13-7-7-7l1.05 1.75"
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
			d="M16.92 22a5.08 5.08 0 1 1 .001-10.162A5.08 5.08 0 0 1 16.92 22ZM5.02 2h3.92c2.07 0 3.07 1 3.02 3.02v3.92c.05 2.07-.95 3.07-3.02 3.02H5.02C3 12 2 11 2 8.93V5.01C2 3 3 2 5.02 2Z"
			:fill="color"
		></path>
		<path
			d="M9.01 8.262c-.31 0-.6-.12-.87-.32.25-.4.43-.85.52-1.34H9c.41 0 .75-.34.75-.75s-.34-.75-.75-.75H7.71a.749.749 0 0 0-.74-.68c-.39 0-.7.3-.74.68H4.94c-.41 0-.75.34-.75.75s.34.75.75.75h2.17c-.3.96-1.16 1.66-2.18 1.66-.41 0-.75.34-.75.75s.34.75.75.75a3.7 3.7 0 0 0 2.18-.72c.55.46 1.21.72 1.89.72.41 0 .75-.34.75-.75s-.33-.75-.74-.75ZM9 22.75c-4.27 0-7.75-3.48-7.75-7.75 0-.41.34-.75.75-.75s.75.34.75.75c0 2.96 2.06 5.44 4.83 6.09l-.27-.45a.751.751 0 1 1 1.29-.77l1.05 1.75c.14.23.14.52.01.75-.14.23-.39.38-.66.38ZM21.998 9.75c-.41 0-.75-.34-.75-.75 0-2.96-2.06-5.44-4.83-6.09l.27.45a.75.75 0 1 1-1.29.77l-1.05-1.75a.745.745 0 0 1-.01-.75c.13-.24.38-.38.65-.38 4.27 0 7.75 3.48 7.75 7.75a.74.74 0 0 1-.74.75ZM19.73 18.33l-2.14-4.27a.77.77 0 0 0-.67-.42.76.76 0 0 0-.67.41l-2.14 4.27c-.19.37-.04.82.34 1.01a.8.8 0 0 0 .33.08c.27 0 .54-.15.67-.41l.17-.34h2.59l.17.34c.19.37.64.52 1.01.34.38-.19.53-.64.34-1.01Zm-3.35-1.17.55-1.09.55 1.09h-1.1Z"
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
			d="m19.06 18.67-2.14-4.27-2.14 4.27M15.17 17.91h3.52"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M16.92 22a5.08 5.08 0 1 1 .002-10.162A5.08 5.08 0 0 1 16.92 22ZM5.02 2h3.92c2.07 0 3.07 1 3.02 3.02v3.92c.05 2.07-.95 3.07-3.02 3.02H5.02C3 12 2 11 2 8.93V5.01C2 3 3 2 5.02 2ZM9.01 5.85H4.95M6.97 5.17v.68"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M7.99 5.84c0 1.75-1.37 3.17-3.05 3.17"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M9.01 9.01c-.73 0-1.39-.39-1.85-1.01M2 15c0 3.87 3.13 7 7 7l-1.05-1.75M22 9c0-3.87-3.13-7-7-7l1.05 1.75"
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
			d="M14.789 19.418c-.11 0-.23-.03-.33-.08a.763.763 0 0 1-.34-1.01l2.14-4.27a.76.76 0 0 1 .67-.41c.28 0 .54.16.67.42l2.14 4.27c.19.37.04.82-.34 1.01-.37.19-.82.04-1.01-.34l-1.46-2.93-1.46 2.93a.78.78 0 0 1-.68.41Z"
			:fill="color"
		></path>
		<path
			d="M18.68 18.66h-3.52c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h3.52a.749.749 0 1 1 0 1.5Z"
			:fill="color"
		></path>
		<path
			d="M16.92 22.75a5.83 5.83 0 1 1 0-11.66 5.83 5.83 0 0 1 0 11.66Zm0-10.15c-2.39 0-4.33 1.94-4.33 4.33s1.94 4.33 4.33 4.33c2.38 0 4.33-1.94 4.33-4.33s-1.94-4.33-4.33-4.33ZM4.86 12.698c-1.11 0-1.99-.31-2.61-.91-.66-.64-1-1.61-1-2.86v-3.92c0-2.43 1.34-3.77 3.77-3.77h3.92c1.25 0 2.21.33 2.86 1 .63.65.94 1.59.91 2.79v3.9c.03 1.22-.28 2.18-.93 2.83-.65.65-1.61.95-2.85.93h-3.9c-.07.01-.12.01-.17.01Zm.16-9.95c-1.61 0-2.27.66-2.27 2.27v3.92c0 .83.18 1.43.54 1.78.35.34.91.49 1.7.48h3.94c.84.02 1.42-.15 1.77-.5.35-.35.51-.94.49-1.75v-3.94c.02-.8-.14-1.37-.48-1.72-.35-.36-.95-.54-1.78-.54H5.02Z"
			:fill="color"
		></path>
		<path
			d="M9.001 6.602h-4.06c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h4.06a.749.749 0 1 1 0 1.5Z"
			:fill="color"
		></path>
		<path
			d="M6.98 6.602c-.41 0-.75-.34-.75-.75v-.68c0-.41.34-.75.75-.75s.75.34.75.75v.68c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M4.941 9.76c-.41 0-.75-.34-.75-.75s.34-.75.75-.75c1.27 0 2.3-1.08 2.3-2.42 0-.41.34-.75.75-.75s.75.34.75.75c0 2.16-1.7 3.92-3.8 3.92Z"
			:fill="color"
		></path>
		<path
			d="M9.01 9.758c-.93 0-1.82-.47-2.45-1.3a.75.75 0 0 1 1.2-.9c.34.46.79.71 1.25.71.41 0 .75.34.75.75s-.34.74-.75.74ZM9 22.75c-4.27 0-7.75-3.48-7.75-7.75 0-.41.34-.75.75-.75s.75.34.75.75c0 2.96 2.06 5.44 4.83 6.09l-.27-.45a.751.751 0 1 1 1.29-.77l1.05 1.75c.14.23.14.52.01.75-.14.23-.39.38-.66.38ZM21.998 9.75c-.41 0-.75-.34-.75-.75 0-2.96-2.06-5.44-4.83-6.09l.27.45a.75.75 0 1 1-1.29.77l-1.05-1.75a.745.745 0 0 1-.01-.75c.13-.24.38-.38.65-.38 4.27 0 7.75 3.48 7.75 7.75a.74.74 0 0 1-.74.75Z"
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
			d="m19.061 18.668-2.14-4.27-2.14 4.27M15.172 17.91h3.52"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M16.92 22a5.08 5.08 0 1 1 .001-10.162A5.08 5.08 0 0 1 16.92 22ZM5.02 2h3.92c2.07 0 3.07 1 3.02 3.02v3.92c.05 2.07-.95 3.07-3.02 3.02H5.02C3 12 2 11 2 8.93V5.01C2 3 3 2 5.02 2ZM9.013 5.852h-4.06M6.973 5.172v.68"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M7.991 5.844c0 1.75-1.37 3.17-3.05 3.17"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M9.01 9.01c-.73 0-1.39-.39-1.85-1.01"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M2 15c0 3.87 3.13 7 7 7l-1.05-1.75M22 9c0-3.87-3.13-7-7-7l1.05 1.75"
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
	name: 'TranslateIcon',
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
