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
			d="M9.001 10.381a2.38 2.38 0 1 0 0-4.76 2.38 2.38 0 0 0 0 4.76Z"
			:fill="color"
		></path>
		<path
			d="M20.97 8h-.47v4.61l-.13-.11c-.78-.67-2.04-.67-2.82 0l-4.16 3.57c-.78.67-2.04.67-2.82 0l-.34-.28c-.71-.62-1.84-.68-2.64-.14l-3.74 2.51c-.22-.56-.35-1.21-.35-1.97V7.81c0-2.82 1.49-4.31 4.31-4.31H16v-.47c0-.4.07-.74.23-1.03H7.81C4.17 2 2 4.17 2 7.81v8.38c0 1.09.19 2.04.56 2.84.86 1.9 2.7 2.97 5.25 2.97h8.38c3.64 0 5.81-2.17 5.81-5.81V7.77c-.29.16-.63.23-1.03.23Z"
			:fill="color"
		></path>
		<path
			d="M20.97 1h-2.94c-.87 0-1.51.36-1.8 1-.16.29-.23.63-.23 1.03V5.97C16 7.24 16.76 8 18.03 8H20.97c.4 0 .74-.07 1.03-.23.64-.29 1-.93 1-1.8V3.03C23 1.76 22.24 1 20.97 1Zm-.67 5.21c-.32.19-.63.29-.8.29-.45 0-1.73-.62-2.11-1.82a1.836 1.836 0 0 1-.02-1.07c.13-.47.44-.88.96-1.05.2-.06.41-.08.6-.04.2.03.39.11.56.24.32-.25.76-.33 1.18-.2.91.3 1.2 1.33.94 2.12-.04.12-.09.24-.15.35-.27.54-.73.94-1.16 1.18Z"
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
			d="M9 6c-1.1 0-2 .9-2 2s.9 2 2 2 2-.9 2-2M2 12.98V15c0 5 2 7 7 7h6c5 0 7-2 7-7v-4M12 2H9C4 2 2 4 2 9M16.122 5.111c-.33-1.04.06-2.33 1.14-2.68.57-.18 1.28-.03 1.68.52.38-.57 1.11-.71 1.68-.52 1.09.35 1.48 1.64 1.15 2.68-.52 1.64-2.32 2.5-2.82 2.5-.51 0-2.3-.84-2.83-2.5Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m2.672 18.949 4.93-3.31c.79-.53 1.93-.47 2.64.14l.33.29c.78.67 2.04.67 2.82 0l4.16-3.57c.78-.67 2.04-.67 2.82 0l1.63 1.4"
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
			d="M21.999 13.899v2.29c0 3.64-2.17 5.81-5.81 5.81h-8.38c-2.55 0-4.39-1.07-5.25-2.97l.11-.08 4.92-3.3c.8-.54 1.93-.48 2.64.14l.34.28c.78.67 2.04.67 2.82 0l4.16-3.57c.78-.67 2.04-.67 2.82 0l1.63 1.4ZM20.97 1h-2.94C16.76 1 16 1.76 16 3.03v2.94C16 7.24 16.76 8 18.03 8h2.94C22.24 8 23 7.24 23 5.97V3.03C23 1.76 22.24 1 20.97 1Zm.64 3.68c-.37 1.18-1.66 1.82-2.11 1.82-.45 0-1.73-.62-2.11-1.82-.06-.18-.09-.38-.09-.57 0-.65.33-1.32 1.02-1.54.41-.13.85-.06 1.16.2.32-.25.76-.33 1.18-.2.92.29 1.21 1.32.95 2.11Z"
			:fill="color"
		></path>
		<path
			opacity=".4"
			d="M20.97 8h-2.94C16.76 8 16 7.24 16 5.97V3.03c0-.4.08-.74.22-1.03H7.81C4.17 2 2 4.17 2 7.81v8.38c0 1.09.19 2.04.56 2.84l.11-.08 4.92-3.3c.8-.54 1.93-.48 2.64.14l.34.28c.78.67 2.04.67 2.82 0l4.16-3.57c.78-.67 2.04-.67 2.82 0L22 13.9V7.78c-.29.14-.63.22-1.03.22Z"
			:fill="color"
		></path>
		<path
			d="M9.001 10.381a2.38 2.38 0 1 0 0-4.76 2.38 2.38 0 0 0 0 4.76Z"
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
			d="M9 10a2 2 0 1 0 0-4 2 2 0 0 0 0 4Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M12 2H9C4 2 2 4 2 9v6c0 5 2 7 7 7h6c5 0 7-2 7-7v-4"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M16.12 5.11c-.33-1.04.06-2.33 1.14-2.68.57-.18 1.28-.03 1.68.52.38-.57 1.11-.71 1.68-.52 1.09.35 1.48 1.64 1.15 2.68-.52 1.64-2.32 2.5-2.82 2.5-.51 0-2.3-.84-2.83-2.5ZM2.67 18.95l4.93-3.31c.79-.53 1.93-.47 2.64.14l.33.29c.78.67 2.04.67 2.82 0l4.16-3.57c.78-.67 2.04-.67 2.82 0L22 13.9"
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
			d="M9 10.75c-1.52 0-2.75-1.23-2.75-2.75S7.48 5.25 9 5.25 11.75 6.48 11.75 8 10.52 10.75 9 10.75Zm0-4a1.25 1.25 0 1 0 0 2.5 1.25 1.25 0 0 0 0-2.5Z"
			:fill="color"
		></path>
		<path
			d="M15 22.75H9c-5.43 0-7.75-2.32-7.75-7.75V9c0-5.43 2.32-7.75 7.75-7.75h3c.41 0 .75.34.75.75s-.34.75-.75.75H9C4.39 2.75 2.75 4.39 2.75 9v6c0 4.61 1.64 6.25 6.25 6.25h6c4.61 0 6.25-1.64 6.25-6.25v-4c0-.41.34-.75.75-.75s.75.34.75.75v4c0 5.43-2.32 7.75-7.75 7.75Z"
			:fill="color"
		></path>
		<path
			d="M18.942 8.358c-.87 0-2.91-1.07-3.54-3.02-.43-1.35.07-3.12 1.63-3.62.66-.21 1.35-.12 1.9.22.54-.34 1.25-.44 1.92-.22 1.56.5 2.06 2.27 1.63 3.62-.63 1.99-2.77 3.02-3.54 3.02Zm-2.11-3.48c.43 1.33 1.87 1.95 2.13 1.98.29-.03 1.7-.73 2.09-1.98.21-.67 0-1.52-.66-1.74-.28-.09-.65-.04-.82.22-.14.21-.37.34-.61.34-.23 0-.48-.11-.62-.31-.21-.29-.58-.33-.84-.25-.67.22-.88 1.07-.67 1.74ZM2.669 19.699a.746.746 0 0 1-.41-1.37l4.93-3.31c1.08-.73 2.57-.64 3.55.19l.33.29c.5.43 1.35.43 1.84 0l4.16-3.57c1.06-.91 2.73-.91 3.8 0l1.63 1.4c.31.27.35.74.08 1.06-.27.31-.74.35-1.06.08l-1.63-1.4c-.5-.43-1.35-.43-1.85 0l-4.16 3.57c-1.06.91-2.73.91-3.8 0l-.33-.29c-.46-.39-1.22-.43-1.73-.08l-4.93 3.31c-.13.08-.28.12-.42.12Z"
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
			d="M9 10a2 2 0 1 0 0-4 2 2 0 0 0 0 4Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M12 2H9C4 2 2 4 2 9v6c0 5 2 7 7 7h6c5 0 7-2 7-7v-4"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M16.122 5.111c-.33-1.04.06-2.33 1.14-2.68.57-.18 1.28-.03 1.68.52.38-.57 1.11-.71 1.68-.52 1.09.35 1.48 1.64 1.15 2.68-.52 1.64-2.32 2.5-2.82 2.5-.51 0-2.3-.84-2.83-2.5ZM2.672 18.949l4.93-3.31c.79-.53 1.93-.47 2.64.14l.33.29c.78.67 2.04.67 2.82 0l4.16-3.57c.78-.67 2.04-.67 2.82 0l1.63 1.4"
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
	name: 'GalleryFavoriteIcon',
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
