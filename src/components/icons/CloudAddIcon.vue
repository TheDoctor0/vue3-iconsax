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
			d="M12 11.531c-2.76 0-5 2.24-5 5 0 .74.16 1.44.46 2.06.08.18.17.35.27.51a4.961 4.961 0 0 0 4.27 2.43c1.82 0 3.41-.98 4.27-2.43.1-.16.19-.33.27-.51.3-.62.46-1.32.46-2.06 0-2.76-2.24-5-5-5Zm2.07 4.57-2.13 1.97c-.14.13-.33.2-.51.2-.19 0-.38-.07-.53-.22l-.99-.99a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l.48.48 1.6-1.48c.31-.28.78-.26 1.06.04s.26.77-.04 1.06Z"
			:fill="color"
		></path>
		<path
			d="M20.2 17.072c-.36.32-.75.59-1.17.81-.36.18-.72-.17-.66-.57.04-.29.06-.59.06-.9 0-3.58-2.92-6.5-6.5-6.5s-6.5 2.92-6.5 6.5c0 .46.05.9.14 1.33.07.35-.2.7-.55.61-3.95-.96-3.97-7.04.45-7.35h.05c-3.21-8.93 10.33-12.5 11.88-3.12 4.33.55 6.08 6.32 2.8 9.19Z"
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
			d="M5.54 11.117c-4.68.33-4.68 7.14 0 7.47h1.92M17.47 8c4.33.55 6.08 6.32 2.8 9.19-1 .91-2.29 1.41-3.64 1.4h-.09M5.589 11.119c-2.53-7.03 5.33-10.74 9.54-7.42"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M17 16.531c0 .74-.16 1.44-.46 2.06-.08.18-.17.35-.27.51a4.961 4.961 0 0 1-4.27 2.43c-1.82 0-3.41-.98-4.27-2.43-.1-.16-.19-.33-.27-.51-.3-.62-.46-1.32-.46-2.06 0-2.76 2.24-5 5-5s5 2.24 5 5Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m10.44 16.53.99.99 2.13-1.97"
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
			d="M20.27 17.189c-1 .91-2.29 1.41-3.64 1.4h-.09c.3-.62.46-1.32.46-2.06 0-2.76-2.24-5-5-5s-5 2.24-5 5c0 .74.16 1.44.46 2.06H5.54c-4.68-.33-4.68-7.14 0-7.47h.05c-3.21-8.93 10.33-12.5 11.88-3.12 4.33.55 6.08 6.32 2.8 9.19Z"
			:fill="color"
		></path>
		<path
			d="M12 11.531c-2.76 0-5 2.24-5 5 0 .74.16 1.44.46 2.06.08.18.17.35.27.51a4.961 4.961 0 0 0 4.27 2.43c1.82 0 3.41-.98 4.27-2.43.1-.16.19-.33.27-.51.3-.62.46-1.32.46-2.06 0-2.76-2.24-5-5-5Zm2.07 4.57-2.13 1.97c-.14.13-.33.2-.51.2-.19 0-.38-.07-.53-.22l-.99-.99a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l.48.48 1.6-1.48c.31-.28.78-.26 1.06.04s.26.77-.04 1.06Z"
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
			d="M5.54 11.12c-4.68.33-4.68 7.14 0 7.47h1.92M5.59 11.12C2.38 2.19 15.92-1.38 17.47 8c4.33.55 6.08 6.32 2.8 9.19-1 .91-2.29 1.41-3.64 1.4h-.09"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M17 16.53c0 .74-.16 1.44-.46 2.06-.08.18-.17.35-.27.51A4.961 4.961 0 0 1 12 21.53c-1.82 0-3.41-.98-4.27-2.43-.1-.16-.19-.33-.27-.51-.3-.62-.46-1.32-.46-2.06 0-2.76 2.24-5 5-5s5 2.24 5 5Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m10.44 16.53.99.99 2.13-1.97"
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
			d="M7.461 19.338h-1.92c-2.94-.21-4.26-2.47-4.26-4.48 0-2.01 1.32-4.28 4.21-4.48.41-.04.77.28.8.7a.75.75 0 0 1-.7.8c-1.94.14-2.81 1.6-2.81 2.99 0 1.39.87 2.85 2.81 2.99h1.87c.41 0 .75.34.75.75s-.34.73-.75.73Z"
			:fill="color"
		></path>
		<path
			d="M16.67 19.339h-.05c-.41 0-.79-.34-.79-.75 0-.43.32-.75.74-.75 1.23 0 2.33-.43 3.19-1.2 1.56-1.36 1.66-3.32 1.24-4.7-.42-1.37-1.59-2.94-3.63-3.19a.753.753 0 0 1-.65-.62c-.4-2.4-1.69-4.06-3.65-4.66-2.02-.63-4.38-.01-5.85 1.53-1.43 1.49-1.76 3.58-.93 5.88a.75.75 0 1 1-1.41.51c-1.01-2.82-.55-5.52 1.26-7.42 1.85-1.94 4.82-2.71 7.37-1.93 2.34.72 3.99 2.65 4.59 5.33 2.04.46 3.68 2.01 4.33 4.15.71 2.33.07 4.73-1.68 6.25-1.11 1-2.56 1.57-4.08 1.57Z"
			:fill="color"
		></path>
		<path
			d="M12 22.281c-2.01 0-3.89-1.07-4.92-2.8-.11-.17-.22-.37-.31-.59-.34-.71-.52-1.52-.52-2.36 0-3.17 2.58-5.75 5.75-5.75s5.75 2.58 5.75 5.75a5.4 5.4 0 0 1-.54 2.39c-.08.19-.19.39-.31.58a5.712 5.712 0 0 1-4.9 2.78Zm0-10a4.26 4.26 0 0 0-4.25 4.25c0 .62.13 1.2.38 1.73.08.17.15.31.23.44a4.227 4.227 0 0 0 3.63 2.08c1.48 0 2.87-.79 3.62-2.06.09-.15.17-.29.23-.43.27-.55.4-1.13.4-1.75.01-2.35-1.9-4.26-4.24-4.26Z"
			:fill="color"
		></path>
		<path
			d="M11.429 18.269c-.19 0-.38-.07-.53-.22l-.99-.99a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l.48.48 1.6-1.48c.31-.28.78-.26 1.06.04s.26.78-.04 1.06l-2.13 1.97c-.15.13-.33.2-.51.2Z"
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
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		>
			<path
				d="M5.54 11.117c-4.68.33-4.68 7.14 0 7.47h1.92M5.59 11.119c-3.21-8.93 10.33-12.5 11.88-3.12 4.33.55 6.08 6.32 2.8 9.19-1 .91-2.29 1.41-3.64 1.4h-.09"
			></path>
		</g>
		<path
			d="M17 16.531c0 .74-.16 1.44-.46 2.06-.08.18-.17.35-.27.51a4.961 4.961 0 0 1-4.27 2.43c-1.82 0-3.41-.98-4.27-2.43-.1-.16-.19-.33-.27-.51-.3-.62-.46-1.32-.46-2.06 0-2.76 2.24-5 5-5s5 2.24 5 5Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m10.44 16.53.99.99 2.13-1.97"
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
	name: 'CloudAddIcon',
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
