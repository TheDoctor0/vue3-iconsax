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
			opacity=".4"
			d="M20.712 17.52c-.37 1.22-1.1 2.16-2.14 2.74-.04-.16-.06-.33-.06-.5 0-1.22.99-2.22 2.2-2.24Z"
			:fill="color"
		></path>
		<path
			d="M21 7.52v1.964c0 .523-.414.945-.92 1.076l-2.95.82c-1.56.4-2.6 1.75-2.6 3.36v1.545c0 .474-.343.87-.769 1.08-1.015.497-1.791 1.506-2.084 2.646-.137.535-.575.989-1.127.989H7.52C4.07 21 2 18.94 2 15.48V7.52C2 4.06 4.07 2 7.52 2h7.96C18.93 2 21 4.06 21 7.52Z"
			:fill="color"
		></path>
		<path
			d="M22.31 12.251c-.26-.19-.68-.39-1.31-.33-.16.01-.33.04-.52.09l-2.98.82c-.89.23-1.47.98-1.47 1.91v3.91c-.23-.08-.48-.13-.74-.13-1.24 0-2.25 1-2.25 2.24 0 .08 0 .16.01.24.12 1.12 1.08 2 2.24 2 1.22 0 2.21-.99 2.23-2.2 0-.02.01-.03.01-.04v-3.69l3.45-.95.52-.14v1.68c-.23-.08-.48-.14-.75-.14h-.04c-1.21.02-2.2 1.02-2.2 2.24 0 .17.02.34.06.5.23 1 1.12 1.75 2.18 1.75 1.23 0 2.22-.99 2.24-2.21 0-.01.01-.02.01-.04v-5.83c0-.76-.23-1.32-.69-1.68Zm-7.02 9.25c-.33 0-.61-.21-.7-.5a.494.494 0 0 1-.05-.24.745.745 0 0 1 1.49 0c0 .08-.01.15-.04.22-.09.3-.37.52-.7.52Zm5.46-.99c-.4 0-.74-.34-.74-.75 0-.4.34-.74.74-.74.41 0 .75.34.75.74 0 .41-.34.75-.75.75Z"
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
			d="M2 12.98V15c0 5 2 7 7 7h2M22 10V9c0-5-2-7-7-7H9C4 2 2 4 2 9M15.268 22.001a1.44 1.44 0 1 0 0-2.88 1.44 1.44 0 0 0 0 2.88Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 19.6v-5.64c0-1.2-.75-1.37-1.52-1.16l-2.89.79c-.52.14-.89.56-.89 1.16v5.82"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M20.557 21.04a1.44 1.44 0 1 0 0-2.88 1.44 1.44 0 0 0 0 2.88ZM16.707 16.428l5.29-1.44"
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
			d="M20.712 17.52c-.37 1.22-1.1 2.16-2.14 2.74-.04-.16-.06-.33-.06-.5 0-1.22.99-2.22 2.2-2.24Z"
			:fill="color"
		></path>
		<path
			opacity=".4"
			d="M21 7.52v7.96c0 .22-.01.43-.02.64l-3.45.95v3.64c-.47.15-.98.24-1.54.27.03-.07.04-.14.04-.22a.745.745 0 0 0-1.49 0c0 .08.01.17.05.24H7.52C4.07 21 2 18.94 2 15.48V7.52C2 4.06 4.07 2 7.52 2h7.96C18.93 2 21 4.06 21 7.52Z"
			:fill="color"
		></path>
		<path
			d="M22.31 12.251c-.26-.19-.68-.39-1.31-.33-.16.01-.33.04-.52.09l-2.98.82c-.89.23-1.47.98-1.47 1.91v3.91c-.23-.08-.48-.13-.74-.13-1.24 0-2.25 1-2.25 2.24 0 .08 0 .16.01.24.12 1.12 1.08 2 2.24 2 1.22 0 2.21-.99 2.23-2.2 0-.02.01-.03.01-.04v-3.69l3.45-.95.52-.14v1.68c-.23-.08-.48-.14-.75-.14h-.04c-1.21.02-2.2 1.02-2.2 2.24 0 .17.02.34.06.5.23 1 1.12 1.75 2.18 1.75 1.23 0 2.22-.99 2.24-2.21 0-.01.01-.02.01-.04v-5.83c0-.76-.23-1.32-.69-1.68Zm-7.02 9.25c-.33 0-.61-.21-.7-.5a.494.494 0 0 1-.05-.24.745.745 0 0 1 1.49 0c0 .08-.01.15-.04.22-.09.3-.37.52-.7.52Zm5.46-.99c-.4 0-.74-.34-.74-.75 0-.4.34-.74.74-.74.41 0 .75.34.75.74 0 .41-.34.75-.75.75Z"
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
			d="M22 10V9c0-5-2-7-7-7H9C4 2 2 4 2 9v6c0 5 2 7 7 7h2M15.27 22a1.44 1.44 0 1 0 0-2.88 1.44 1.44 0 0 0 0 2.88Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 19.6v-5.64c0-1.2-.75-1.37-1.52-1.16l-2.89.79c-.52.14-.89.56-.89 1.16v5.82"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M20.56 21.04a1.44 1.44 0 1 0 0-2.88 1.44 1.44 0 0 0 0 2.88ZM16.71 16.43 22 14.99"
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
			d="M11 22.75H9c-5.43 0-7.75-2.32-7.75-7.75V9c0-5.43 2.32-7.75 7.75-7.75h6c5.43 0 7.75 2.32 7.75 7.75v1c0 .41-.34.75-.75.75s-.75-.34-.75-.75V9c0-4.61-1.64-6.25-6.25-6.25H9C4.39 2.75 2.75 4.39 2.75 9v6c0 4.61 1.64 6.25 6.25 6.25h2c.41 0 .75.34.75.75s-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M15.268 22.751a2.19 2.19 0 1 1-.001-4.379 2.19 2.19 0 0 1 .001 4.38Zm0-2.89c-.38 0-.69.31-.69.69 0 .38.31.69.69.69.38 0 .69-.31.69-.69 0-.38-.31-.69-.69-.69Z"
			:fill="color"
		></path>
		<path
			d="M16.71 21.31c-.41 0-.75-.34-.75-.75v-5.82c0-.91.56-1.65 1.44-1.88l2.89-.79c.9-.25 1.46-.01 1.78.23.31.24.68.72.68 1.65v5.64c0 .41-.34.75-.75.75s-.75-.34-.75-.75v-5.64c0-.32-.07-.44-.1-.46-.03-.02-.17-.06-.48.02l-2.89.79c-.3.08-.33.29-.33.44v5.82a.74.74 0 0 1-.74.75Z"
			:fill="color"
		></path>
		<path
			d="M20.561 21.79a2.19 2.19 0 1 1-.001-4.379 2.19 2.19 0 0 1 .001 4.38Zm0-2.89c-.38 0-.69.31-.69.69 0 .38.31.69.69.69.38 0 .69-.31.69-.69 0-.38-.31-.69-.69-.69ZM16.712 17.179a.747.747 0 0 1-.19-1.47l5.29-1.44a.75.75 0 1 1 .39 1.45l-5.29 1.44c-.07.01-.14.02-.2.02Z"
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
			d="M22 10V9c0-5-2-7-7-7H9C4 2 2 4 2 9v6c0 5 2 7 7 7h2"
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
			<path
				d="M15.268 22.001a1.44 1.44 0 1 0 0-2.88 1.44 1.44 0 0 0 0 2.88Z"
			></path>
			<path
				d="M22 19.6v-5.64c0-1.2-.75-1.37-1.52-1.16l-2.89.79c-.52.14-.89.56-.89 1.16v5.82"
			></path>
			<path
				d="M20.557 21.04a1.44 1.44 0 1 0 0-2.88 1.44 1.44 0 0 0 0 2.88ZM16.707 16.428l5.29-1.44"
			></path>
		</g>
	</svg>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
	name: 'MiniMusicSqaureIcon',
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
