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
			d="M5 15c-2.21 0-4 1.79-4 4 0 .75.21 1.46.58 2.06A3.97 3.97 0 0 0 5 23c1.46 0 2.73-.78 3.42-1.94.37-.6.58-1.31.58-2.06 0-2.21-1.79-4-4-4Zm1.97 3.67-2.13 1.97c-.14.13-.33.2-.51.2-.19 0-.38-.07-.53-.22l-.99-.99a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l.48.48 1.6-1.48c.3-.28.78-.26 1.06.04s.26.78-.04 1.06ZM21.5 12.5H19c-1.1 0-2 .9-2 2s.9 2 2 2h2.5c.28 0 .5-.22.5-.5v-3c0-.28-.22-.5-.5-.5ZM16.53 5.4c.3.29.05.74-.37.74l-8.28-.01c-.48 0-.72-.58-.38-.92l1.75-1.76a3.796 3.796 0 0 1 5.35 0l1.89 1.91.04.04Z"
			:fill="color"
		></path>
		<path
			d="M21.87 18.66C21.26 20.72 19.5 22 17.1 22h-6.5c-.39 0-.64-.43-.48-.79.3-.7.49-1.49.49-2.21 0-3.03-2.47-5.5-5.5-5.5-.76 0-1.5.16-2.18.46-.37.16-.82-.09-.82-.49V12c0-2.72 1.64-4.62 4.19-4.94.25-.04.52-.06.8-.06h10c.26 0 .51.01.75.05 2.02.23 3.48 1.46 4.02 3.29.1.33-.14.66-.48.66H19.1c-2.17 0-3.89 1.98-3.42 4.23.33 1.64 1.85 2.77 3.52 2.77h2.19c.35 0 .58.34.48.66Z"
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
			d="M6.19 7.06C6.45 7.02 6.72 7 7 7h10c.26 0 .51.01.75.05C20.33 7.35 22 9.26 22 12v5c0 3-2 5-5 5H7.63c.31-.26.58-.58.79-.94.37-.6.58-1.31.58-2.06 0-2.21-1.79-4-4-4-1.2 0-2.27.53-3 1.36V12c0-.87.17-1.66.48-2.33"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M9 19c0 .75-.21 1.46-.58 2.06A3.97 3.97 0 0 1 5 23a3.97 3.97 0 0 1-3.42-1.94A3.92 3.92 0 0 1 1 19c0-2.21 1.79-4 4-4s4 1.79 4 4Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m3.441 19 .99.99 2.13-1.97M17.751 7.05c-.24-.04-.49-.05-.75-.05h-10c-.28 0-.55.02-.81.06.14-.28.34-.54.58-.78l3.25-3.26a3.525 3.525 0 0 1 4.96 0l1.75 1.77c.64.63.98 1.43 1.02 2.26ZM22 12.5h-3c-1.1 0-2 .9-2 2s.9 2 2 2h3"
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
			d="M5 15c-2.21 0-4 1.79-4 4 0 .75.21 1.46.58 2.06A3.97 3.97 0 0 0 5 23c1.46 0 2.73-.78 3.42-1.94.37-.6.58-1.31.58-2.06 0-2.21-1.79-4-4-4Zm1.97 3.67-2.13 1.97c-.14.13-.33.2-.51.2-.19 0-.38-.07-.53-.22l-.99-.99a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l.48.48 1.6-1.48c.3-.28.78-.26 1.06.04s.26.78-.04 1.06ZM17.751 7.05c-.24-.04-.49-.05-.75-.05h-10c-.28 0-.55.02-.81.06.14-.28.34-.54.58-.78l3.25-3.26a3.525 3.525 0 0 1 4.96 0l1.75 1.77c.64.63.98 1.43 1.02 2.26Z"
			:fill="color"
		></path>
		<path
			opacity=".4"
			d="M22 12v5c0 3-2 5-5 5H7.63c.31-.26.58-.58.79-.94.37-.6.58-1.31.58-2.06 0-2.21-1.79-4-4-4-1.2 0-2.27.53-3 1.36V12c0-2.72 1.64-4.62 4.19-4.94.26-.04.53-.06.81-.06h10c.26 0 .51.01.75.05C20.33 7.35 22 9.26 22 12Z"
			:fill="color"
		></path>
		<path
			d="M22 12.5h-3c-1.1 0-2 .9-2 2s.9 2 2 2h3"
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
			d="M9 19c0 .75-.21 1.46-.58 2.06A3.97 3.97 0 0 1 5 23a3.97 3.97 0 0 1-3.42-1.94A3.92 3.92 0 0 1 1 19c0-2.21 1.79-4 4-4s4 1.79 4 4Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m3.441 19 .99.99 2.13-1.97M17.751 7.05c-.24-.04-.49-.05-.75-.05h-10c-.28 0-.55.02-.81.06.14-.28.34-.54.58-.78l3.25-3.26a3.525 3.525 0 0 1 4.96 0l1.75 1.77c.64.63.98 1.43 1.02 2.26Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 12v5c0 3-2 5-5 5H7.63c.31-.26.58-.58.79-.94.37-.6.58-1.31.58-2.06 0-2.21-1.79-4-4-4-1.2 0-2.27.53-3 1.36V12c0-2.72 1.64-4.62 4.19-4.94.26-.04.53-.06.81-.06h10c.26 0 .51.01.75.05C20.33 7.35 22 9.26 22 12Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 12.5h-3c-1.1 0-2 .9-2 2s.9 2 2 2h3"
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
			d="M5 23.75c-1.66 0-3.22-.88-4.06-2.31C.49 20.72.25 19.87.25 19c0-2.62 2.13-4.75 4.75-4.75S9.75 16.38 9.75 19c0 .87-.24 1.72-.69 2.45-.84 1.42-2.4 2.3-4.06 2.3Zm0-8c-1.79 0-3.25 1.46-3.25 3.25 0 .59.16 1.17.47 1.67.59 1 1.63 1.58 2.78 1.58s2.19-.59 2.78-1.57c.31-.51.47-1.08.47-1.68 0-1.79-1.46-3.25-3.25-3.25Z"
			:fill="color"
		></path>
		<path
			d="M4.429 20.741c-.19 0-.38-.07-.53-.22l-.99-.99a.755.755 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l.48.48 1.6-1.48c.3-.28.78-.26 1.06.04s.26.78-.04 1.06l-2.13 1.97c-.15.13-.33.2-.51.2ZM6.192 7.811c-.24 0-.46-.11-.61-.31a.735.735 0 0 1-.06-.78c.17-.34.41-.67.72-.97l3.25-3.26a4.28 4.28 0 0 1 6.02 0l1.75 1.78c.74.73 1.19 1.71 1.24 2.75a.752.752 0 0 1-.87.78c-.2-.03-.41-.04-.63-.04h-10c-.24 0-.47.02-.7.05h-.11Zm1.67-1.56h8.96c-.13-.34-.34-.65-.62-.93l-1.76-1.78c-1.07-1.06-2.82-1.06-3.9 0l-2.68 2.71Z"
			:fill="color"
		></path>
		<path
			d="M17 22.75H7.63c-.32 0-.6-.2-.71-.49-.11-.3-.02-.63.22-.83.24-.2.46-.46.62-.74.32-.51.48-1.09.48-1.68 0-1.79-1.46-3.25-3.25-3.25-.93 0-1.82.4-2.44 1.11-.21.23-.54.32-.83.21a.757.757 0 0 1-.49-.7V12c0-3.08 1.9-5.31 4.85-5.68.27-.04.58-.07.9-.07h10c.24 0 .55.01.87.06 2.95.34 4.88 2.58 4.88 5.69v5c.02 3.44-2.29 5.75-5.73 5.75Zm-7.82-1.5H17c2.58 0 4.25-1.67 4.25-4.25v-5c0-2.34-1.37-3.95-3.59-4.21-.24-.04-.45-.04-.66-.04H7c-.24 0-.47.02-.7.05-2.2.28-3.55 1.88-3.55 4.2v2.82c.68-.37 1.46-.57 2.25-.57 2.62 0 4.75 2.13 4.75 4.75 0 .79-.2 1.57-.57 2.25Z"
			:fill="color"
		></path>
		<path
			d="M22 17.25h-3c-1.52 0-2.75-1.23-2.75-2.75s1.23-2.75 2.75-2.75h3c.41 0 .75.34.75.75s-.34.75-.75.75h-3a1.25 1.25 0 0 0 0 2.5h3c.41 0 .75.34.75.75s-.34.75-.75.75Z"
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
			d="M9 19c0 .75-.21 1.46-.58 2.06A3.97 3.97 0 0 1 5 23a3.97 3.97 0 0 1-3.42-1.94A3.92 3.92 0 0 1 1 19c0-2.21 1.79-4 4-4s4 1.79 4 4Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m3.441 19 .99.99 2.13-1.97"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M17.751 7.05c-.24-.04-.49-.05-.75-.05h-10c-.28 0-.55.02-.81.06.14-.28.34-.54.58-.78l3.25-3.26a3.525 3.525 0 0 1 4.96 0l1.75 1.77c.64.63.98 1.43 1.02 2.26Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 12v5c0 3-2 5-5 5H7.63c.31-.26.58-.58.79-.94.37-.6.58-1.31.58-2.06 0-2.21-1.79-4-4-4-1.2 0-2.27.53-3 1.36V12c0-2.72 1.64-4.62 4.19-4.94.26-.04.53-.06.81-.06h10c.26 0 .51.01.75.05C20.33 7.35 22 9.26 22 12Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M22 12.5h-3c-1.1 0-2 .9-2 2s.9 2 2 2h3"
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
	name: 'WalletCheckIcon',
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
