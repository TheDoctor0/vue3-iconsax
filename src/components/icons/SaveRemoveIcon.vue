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
			d="M22 5.11v11.36c0 1.45-1.04 2.06-2.31 1.36l-1.93-1.08a.509.509 0 0 1-.26-.44V8.99c0-2.54-2.07-4.61-4.61-4.61H8.82c-.37 0-.63-.39-.46-.71C8.88 2.68 9.92 2 11.11 2h7.78C20.6 2 22 3.4 22 5.11Z"
			:fill="color"
		></path>
		<path
			d="M12.89 5.879H5.11A3.12 3.12 0 0 0 2 8.989v11.36c0 1.45 1.04 2.06 2.31 1.36l3.93-2.19c.42-.23 1.1-.23 1.52 0l3.93 2.19c1.27.7 2.31.09 2.31-1.36V8.989c0-1.71-1.4-3.11-3.11-3.11Zm-1.95 7c.29.29.29.77 0 1.06-.15.15-.34.22-.53.22s-.38-.07-.53-.22l-.88-.88-.88.88c-.15.15-.34.22-.53.22s-.38-.07-.53-.22a.754.754 0 0 1 0-1.06l.88-.88-.88-.88a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l.88.88.88-.88c.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06l-.88.88.88.88Z"
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
			d="M2 20.349c0 1.45 1.04 2.06 2.31 1.36l3.93-2.19c.42-.23 1.1-.23 1.52 0l3.93 2.19c1.27.7 2.31.09 2.31-1.36V8.989c0-1.71-1.4-3.11-3.11-3.11H5.11A3.12 3.12 0 0 0 2 8.989v7.58M7.59 13.41l2.82-2.82M10.41 13.41l-2.82-2.82"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 5.11v11.36c0 1.45-1.04 2.06-2.31 1.36L16 15.77V8.99c0-1.71-1.4-3.11-3.11-3.11H8v-.77C8 3.4 9.4 2 11.11 2h7.78C20.6 2 22 3.4 22 5.11Z"
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
			d="M16 8.989v11.36c0 1.45-1.04 2.06-2.31 1.36l-3.93-2.19c-.42-.23-1.1-.23-1.52 0l-3.93 2.19c-1.27.7-2.31.09-2.31-1.36V8.989c0-1.71 1.4-3.11 3.11-3.11h7.78c1.71 0 3.11 1.4 3.11 3.11Z"
			:fill="color"
		></path>
		<path
			d="m10.06 12.001.88-.88c.29-.29.29-.77 0-1.06a.754.754 0 0 0-1.06 0l-.88.88-.88-.88a.754.754 0 0 0-1.06 0c-.29.29-.29.77 0 1.06l.88.88-.88.88c-.29.29-.29.77 0 1.06.15.15.34.22.53.22s.38-.07.53-.22l.88-.88.88.88c.15.15.34.22.53.22s.38-.07.53-.22c.29-.29.29-.77 0-1.06l-.88-.88ZM22 5.11v11.36c0 1.45-1.04 2.06-2.31 1.36L16 15.77V8.99c0-1.71-1.4-3.11-3.11-3.11H8v-.77C8 3.4 9.4 2 11.11 2h7.78C20.6 2 22 3.4 22 5.11Z"
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
			d="M16 8.99v11.36c0 1.45-1.04 2.06-2.31 1.36l-3.93-2.19c-.42-.23-1.1-.23-1.52 0l-3.93 2.19c-1.27.7-2.31.09-2.31-1.36V8.99c0-1.71 1.4-3.11 3.11-3.11h7.78c1.71 0 3.11 1.4 3.11 3.11ZM7.59 13.41l2.82-2.82M10.41 13.41l-2.82-2.82"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 5.11v11.36c0 1.45-1.04 2.06-2.31 1.36L16 15.77V8.99c0-1.71-1.4-3.11-3.11-3.11H8v-.77C8 3.4 9.4 2 11.11 2h7.78C20.6 2 22 3.4 22 5.11Z"
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
			d="M14.69 22.75c-.44 0-.9-.13-1.37-.38l-3.93-2.19c-.19-.1-.6-.1-.79 0l-3.93 2.19c-.85.47-1.71.51-2.38.12-.66-.39-1.05-1.17-1.05-2.13V9c0-2.13 1.73-3.86 3.86-3.86h7.78c2.13 0 3.86 1.73 3.86 3.86v11.36c0 .96-.38 1.74-1.05 2.13-.29.17-.63.26-1 .26ZM9 18.6c.4 0 .79.09 1.12.27l3.94 2.19c.36.2.69.25.89.13.19-.11.31-.43.31-.84V8.99c0-1.3-1.06-2.36-2.36-2.36H5.11c-1.3 0-2.36 1.06-2.36 2.36v11.36c0 .41.12.73.31.84.19.11.53.06.89-.14l3.93-2.19c.32-.17.72-.26 1.12-.26Z"
			:fill="color"
		></path>
		<path
			d="M7.59 14.16c-.19 0-.38-.07-.53-.22a.754.754 0 0 1 0-1.06l2.83-2.83c.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06l-2.83 2.83c-.15.15-.34.22-.53.22Z"
			:fill="color"
		></path>
		<path
			d="M10.41 14.16c-.19 0-.38-.07-.53-.22l-2.83-2.83a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l2.83 2.83c.29.29.29.77 0 1.06a.71.71 0 0 1-.53.22ZM20.69 18.872c-.44 0-.9-.13-1.37-.38l-3.69-2.06a.732.732 0 0 1-.38-.65v-6.78c0-1.3-1.06-2.36-2.36-2.36H8c-.41 0-.75-.34-.75-.75v-.77c0-2.13 1.73-3.86 3.86-3.86h7.78c2.13 0 3.86 1.73 3.86 3.86v11.36c0 .96-.38 1.74-1.05 2.13-.3.17-.64.26-1.01.26Zm-3.94-3.54 3.31 1.85c.36.2.69.25.89.13.19-.11.31-.43.31-.84V5.112c0-1.3-1.06-2.36-2.36-2.36h-7.78c-1.3 0-2.36 1.06-2.36 2.36v.02h4.14c2.13 0 3.86 1.73 3.86 3.86v6.34h-.01Z"
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
			d="M16 8.989v11.36c0 1.45-1.04 2.06-2.31 1.36l-3.93-2.19c-.42-.23-1.1-.23-1.52 0l-3.93 2.19c-1.27.7-2.31.09-2.31-1.36V8.989c0-1.71 1.4-3.11 3.11-3.11h7.78c1.71 0 3.11 1.4 3.11 3.11Z"
			:stroke="color"
			:stroke-width="strokeWidth"
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
			<path d="m7.59 13.41 2.82-2.82M10.41 13.41l-2.82-2.82"></path>
		</g>
		<path
			d="M22 5.11v11.36c0 1.45-1.04 2.06-2.31 1.36L16 15.77V8.99c0-1.71-1.4-3.11-3.11-3.11H8v-.77C8 3.4 9.4 2 11.11 2h7.78C20.6 2 22 3.4 22 5.11Z"
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
	name: 'SaveRemoveIcon',
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
