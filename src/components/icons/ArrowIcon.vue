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
			d="M12 22.75c-.41 0-.75-.34-.75-.75v-2c0-.41.34-.75.75-.75s.75.34.75.75v2c0 .41-.34.75-.75.75ZM12 18.75c-.41 0-.75-.34-.75-.75v-2c0-.41.34-.75.75-.75s.75.34.75.75v2c0 .41-.34.75-.75.75ZM12 14.75c-.41 0-.75-.34-.75-.75v-3c0-4.27 3.48-7.75 7.75-7.75h3c.41 0 .75.34.75.75s-.34.75-.75.75h-3c-3.45 0-6.25 2.8-6.25 6.25v3c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M12 14.75c-.41 0-.75-.34-.75-.75v-3c0-3.45-2.8-6.25-6.25-6.25H2c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h3c4.27 0 7.75 3.48 7.75 7.75v3c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M4.001 6.751c-.19 0-.38-.07-.53-.22l-2-2a.754.754 0 0 1 0-1.06l2-2c.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06l-1.47 1.47 1.47 1.47c.29.29.29.77 0 1.06-.15.15-.34.22-.53.22ZM20.001 6.751c-.19 0-.38-.07-.53-.22a.754.754 0 0 1 0-1.06l1.47-1.47-1.47-1.47a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l2 2c.29.29.29.77 0 1.06l-2 2c-.15.15-.34.22-.53.22Z"
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
			d="M12 22v-2M12 18v-2M12 14v-3c0-3.87 3.13-7 7-7h3"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M9.45 5.602a6.973 6.973 0 0 1 2.55 5.4v3M2 4h3M4 2 2 4l2 2M20 2l2 2-2 2"
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
			d="M12 22.75c-.41 0-.75-.34-.75-.75v-2c0-.41.34-.75.75-.75s.75.34.75.75v2c0 .41-.34.75-.75.75ZM12 18.75c-.41 0-.75-.34-.75-.75v-2c0-.41.34-.75.75-.75s.75.34.75.75v2c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M12 14.75c-.41 0-.75-.34-.75-.75v-3c0-4.27 3.48-7.75 7.75-7.75h3c.41 0 .75.34.75.75s-.34.75-.75.75h-3c-3.45 0-6.25 2.8-6.25 6.25v3c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M12 14.75c-.41 0-.75-.34-.75-.75v-3c0-3.45-2.8-6.25-6.25-6.25H2c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h3c4.27 0 7.75 3.48 7.75 7.75v3c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M4.001 6.751c-.19 0-.38-.07-.53-.22l-2-2a.754.754 0 0 1 0-1.06l2-2c.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06l-1.47 1.47 1.47 1.47c.29.29.29.77 0 1.06-.15.15-.34.22-.53.22ZM20.001 6.751c-.19 0-.38-.07-.53-.22a.754.754 0 0 1 0-1.06l1.47-1.47-1.47-1.47a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l2 2c.29.29.29.77 0 1.06l-2 2c-.15.15-.34.22-.53.22Z"
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
			d="M12 22v-2M12 18v-2M12 14v-3c0-3.87 3.13-7 7-7h3M2 4h3c3.87 0 7 3.13 7 7v3"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M4 2 2 4l2 2M20 2l2 2-2 2"
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
			d="M12 22.75c-.41 0-.75-.34-.75-.75v-2c0-.41.34-.75.75-.75s.75.34.75.75v2c0 .41-.34.75-.75.75ZM12 18.75c-.41 0-.75-.34-.75-.75v-2c0-.41.34-.75.75-.75s.75.34.75.75v2c0 .41-.34.75-.75.75ZM12 14.75c-.41 0-.75-.34-.75-.75v-3c0-4.27 3.48-7.75 7.75-7.75h3c.41 0 .75.34.75.75s-.34.75-.75.75h-3c-3.45 0-6.25 2.8-6.25 6.25v3c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M12 14.75c-.41 0-.75-.34-.75-.75v-3c0-3.45-2.8-6.25-6.25-6.25H2c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h3c4.27 0 7.75 3.48 7.75 7.75v3c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M4.001 6.751c-.19 0-.38-.07-.53-.22l-2-2a.754.754 0 0 1 0-1.06l2-2c.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06l-1.47 1.47 1.47 1.47c.29.29.29.77 0 1.06-.15.15-.34.22-.53.22ZM20.001 6.751c-.19 0-.38-.07-.53-.22a.754.754 0 0 1 0-1.06l1.47-1.47-1.47-1.47a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l2 2c.29.29.29.77 0 1.06l-2 2c-.15.15-.34.22-.53.22Z"
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
			:stroke="color"
			stroke-linecap="round"
			stroke-linejoin="round"
			:stroke-width="strokeWidth"
			d="M12 22v-2M12 18v-2"
			opacity=".4"
		></path>
		<path
			:stroke="color"
			stroke-linecap="round"
			stroke-linejoin="round"
			:stroke-width="strokeWidth"
			d="M12 14v-3c0-3.87 3.13-7 7-7h3M2 4h3c3.87 0 7 3.13 7 7v3"
		></path>
		<path
			:stroke="color"
			stroke-linecap="round"
			stroke-linejoin="round"
			:stroke-width="strokeWidth"
			d="M4 2L2 4l2 2M20 2l2 2-2 2"
		></path>
	</svg>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
	name: 'ArrowIcon',
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
