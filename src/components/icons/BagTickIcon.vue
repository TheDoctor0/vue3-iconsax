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
			d="M19.24 5.579h-.4l-3.38-3.38a.706.706 0 0 0-.99 0c-.27.27-.27.71 0 .99l2.39 2.39H7.14l2.39-2.39c.27-.27.27-.71 0-.99a.706.706 0 0 0-.99 0l-3.37 3.38h-.4c-.9 0-2.77 0-2.77 2.56 0 .97.2 1.61.62 2.03.24.25.53.38.84.45.29.07.6.08.9.08h15.28c.31 0 .6-.02.88-.08.84-.2 1.48-.8 1.48-2.48 0-2.56-1.87-2.56-2.76-2.56ZM19.09 12H4.91c-.62 0-1.09.55-.99 1.16l.84 5.14c.28 1.72 1.03 3.7 4.36 3.7h5.61c3.37 0 3.97-1.69 4.33-3.58l1.01-5.23a.997.997 0 0 0-.98-1.19Zm-4.21 4.05-3.25 3c-.14.13-.32.2-.51.2s-.38-.07-.53-.22l-1.5-1.5a.754.754 0 0 1 0-1.06c.3-.29.77-.29 1.07 0l.99.99 2.72-2.51c.3-.28.78-.26 1.06.04.28.31.26.78-.05 1.06Z"
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
			d="m9.62 16 1.5 1.5 3.25-3"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M8.81 2 5.19 5.63M15.19 2l3.62 3.63"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M2 7.852c0-1.85.99-2 2.22-2h15.56c1.23 0 2.22.15 2.22 2 0 2.15-.99 2-2.22 2H4.22c-1.23 0-2.22.15-2.22-2Z"
			:stroke="color"
			:stroke-width="strokeWidth"
		></path>
		<path
			d="M4.91 18.64C5.23 20.58 6 22 8.86 22h6.03c3.11 0 3.57-1.36 3.93-3.24L20.5 10M3.5 10l.69 4.25"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
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
			d="M19.24 5.579h-.4l-3.38-3.38a.706.706 0 0 0-.99 0c-.27.27-.27.71 0 .99l2.39 2.39H7.14l2.39-2.39c.27-.27.27-.71 0-.99a.706.706 0 0 0-.99 0l-3.37 3.38h-.4c-.9 0-2.77 0-2.77 2.56 0 .97.2 1.61.62 2.03.24.25.53.38.84.45.29.07.6.08.9.08h15.28c.31 0 .6-.02.88-.08.84-.2 1.48-.8 1.48-2.48 0-2.56-1.87-2.56-2.76-2.56Z"
			:fill="color"
		></path>
		<path
			d="M19.66 10.7H4.36c-.29 0-.61-.01-.9-.09l1.26 7.69c.29 1.72 1.04 3.7 4.37 3.7h5.61c3.37 0 3.97-1.69 4.33-3.58l1.51-7.81c-.28.07-.58.09-.88.09Zm-4.78 4.35-3.25 3c-.14.13-.33.2-.51.2-.19 0-.38-.07-.53-.22l-1.5-1.5a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l.99.99 2.72-2.51c.3-.28.78-.26 1.06.04.29.31.27.78-.04 1.06Z"
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
			d="m9.62 16 1.5 1.5 3.25-3"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M8.81 2 5.19 5.63M15.19 2l3.62 3.63"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M2 7.85c0-1.85.99-2 2.22-2h15.56c1.23 0 2.22.15 2.22 2 0 2.15-.99 2-2.22 2H4.22C2.99 9.85 2 10 2 7.85Z"
			:stroke="color"
			:stroke-width="strokeWidth"
		></path>
		<path
			d="m3.5 10 1.41 8.64C5.23 20.58 6 22 8.86 22h6.03c3.11 0 3.57-1.36 3.93-3.24L20.5 10"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
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
			d="M11.12 18.248c-.19 0-.38-.07-.53-.22l-1.5-1.5a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l.99.99 2.72-2.51c.3-.28.78-.26 1.06.04s.26.78-.04 1.06l-3.25 3c-.14.13-.32.2-.51.2ZM5.19 6.381c-.19 0-.39-.08-.53-.22a.754.754 0 0 1 0-1.06l3.63-3.63c.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06l-3.63 3.63c-.15.14-.34.22-.53.22ZM18.81 6.381c-.19 0-.38-.07-.53-.22l-3.63-3.63a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l3.63 3.63c.29.29.29.77 0 1.06-.14.14-.34.22-.53.22Z"
			:fill="color"
		></path>
		<path
			d="M20.21 10.602H4c-.7.01-1.5.01-2.08-.57-.46-.45-.67-1.15-.67-2.18 0-2.75 2.01-2.75 2.97-2.75h15.56c.96 0 2.97 0 2.97 2.75 0 1.04-.21 1.73-.67 2.18-.52.52-1.22.57-1.87.57Zm-15.99-1.5h15.79c.45.01.87.01 1.01-.13.07-.07.22-.31.22-1.12 0-1.13-.28-1.25-1.47-1.25H4.22c-1.19 0-1.47.12-1.47 1.25 0 .81.16 1.05.22 1.12.14.13.57.13 1.01.13h.24Z"
			:fill="color"
		></path>
		<path
			d="M14.89 22.75H8.86c-3.58 0-4.38-2.13-4.69-3.98l-1.41-8.65c-.07-.41.21-.79.62-.86.4-.07.79.21.86.62l1.41 8.64c.29 1.77.89 2.73 3.21 2.73h6.03c2.57 0 2.86-.9 3.19-2.64l1.68-8.75c.08-.41.47-.68.88-.59.41.08.67.47.59.88l-1.68 8.75c-.39 2.03-1.04 3.85-4.66 3.85Z"
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
			<path d="m9.62 16 1.5 1.5 3.25-3"></path>
			<path
				d="M8.81 2 5.19 5.63M15.19 2l3.62 3.63"
				stroke-miterlimit="10"
			></path>
		</g>
		<path
			d="M2 7.852c0-1.85.99-2 2.22-2h15.56c1.23 0 2.22.15 2.22 2 0 2.15-.99 2-2.22 2H4.22c-1.23 0-2.22.15-2.22-2Z"
			:stroke="color"
			:stroke-width="strokeWidth"
		></path>
		<path
			d="m3.5 10 1.41 8.64C5.23 20.58 6 22 8.86 22h6.03c3.11 0 3.57-1.36 3.93-3.24L20.5 10"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
		></path>
	</svg>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
	name: 'BagTickIcon',
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
