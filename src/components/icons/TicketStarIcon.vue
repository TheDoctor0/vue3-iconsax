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
			d="M16.649 3.86h-6.74v3.02c0 .39-.32.7-.7.7-.38 0-.7-.31-.7-.7V3.86h-1.16c-3.95 0-5.25 1.18-5.34 4.87-.01.18.07.37.2.5.13.14.3.21.5.21 1.4 0 2.55 1.16 2.55 2.56 0 1.4-1.15 2.56-2.55 2.56-.19 0-.37.07-.5.21-.13.13-.21.32-.2.5.09 3.69 1.39 4.87 5.34 4.87h1.16v-3.02c0-.39.32-.7.7-.7.38 0 .7.31.7.7v3.02h6.74c4.1 0 5.35-1.25 5.35-5.35V9.21c0-4.1-1.25-5.35-5.35-5.35Zm1.82 8.04-.93.9c-.04.03-.05.09-.04.14l.22 1.27c.04.23-.05.47-.25.61-.19.14-.44.16-.65.05l-1.15-.6a.17.17 0 0 0-.14 0l-1.15.6c-.09.05-.19.07-.29.07a.625.625 0 0 1-.61-.73l.22-1.27a.18.18 0 0 0-.04-.14l-.93-.9a.616.616 0 0 1-.16-.63.59.59 0 0 1 .5-.42l1.28-.19a.2.2 0 0 0 .12-.08l.57-1.16c.11-.21.32-.34.56-.34a.6.6 0 0 1 .55.34l.57 1.16c.02.05.06.08.11.08l1.28.19c.24.03.43.2.5.42.09.22.03.46-.14.63Z"
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
			d="M3.242 15.27c-.38.14-.8.22-1.23.22.09 3.59 1.16 4.51 4.99 4.51h10c4 0 5-1 5-5V9c0-4-1-5-5-5h-10c-3.83 0-4.9.92-4.99 4.5 1.93 0 3.49 1.57 3.49 3.5M9 4v3.5M9 16.5V20"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M14.862 14.208a.445.445 0 0 0-.39 0l-1.23.65c-.31.16-.66-.1-.6-.44l.24-1.37a.422.422 0 0 0-.12-.37l-.99-.97a.416.416 0 0 1 .23-.71l1.38-.2c.14-.02.25-.1.31-.23l.61-1.25a.41.41 0 0 1 .74 0l.62 1.25c.06.12.18.21.31.23l1.38.2c.34.05.48.47.23.71l-1 .97c-.1.09-.14.23-.12.37"
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
			d="M22 9.21v5.58c0 4.1-1.25 5.35-5.35 5.35H9.91v-3.02c0-.38-.32-.7-.7-.7V7.58c.38 0 .7-.32.7-.7V3.86h6.74c4.1 0 5.35 1.25 5.35 5.35Z"
			:fill="color"
		></path>
		<path
			d="M18.471 11.898c.17-.16.23-.41.16-.63a.59.59 0 0 0-.5-.42l-1.28-.19a.155.155 0 0 1-.11-.08l-.57-1.16a.61.61 0 0 0-.55-.34c-.24 0-.45.13-.56.34l-.57 1.16a.13.13 0 0 1-.12.08l-1.28.19c-.23.03-.43.2-.5.42a.61.61 0 0 0 .16.63l.93.9c.04.03.05.09.04.14l-.22 1.27c-.04.23.05.47.25.6a.6.6 0 0 0 .36.12c.1 0 .2-.02.29-.07l1.15-.6c.04-.02.1-.02.14 0l1.15.6a.625.625 0 0 0 .9-.66l-.22-1.27a.18.18 0 0 1 .04-.14l.91-.89ZM9.209 7.58v8.84c-.38 0-.7.32-.7.7v3.02h-1.16c-3.95 0-5.25-1.18-5.34-4.86-.01-.19.07-.37.2-.5.13-.14.32-.21.5-.21 1.4 0 2.55-1.15 2.55-2.56 0-1.41-1.15-2.57-2.55-2.57-.2 0-.37-.07-.5-.21a.679.679 0 0 1-.2-.5c.09-3.69 1.39-4.87 5.34-4.87h1.16v3.02c0 .39.32.7.7.7Z"
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
			d="M16.995 4h-10c-3.83 0-4.9.92-4.99 4.5 1.93 0 3.49 1.57 3.49 3.5s-1.56 3.49-3.49 3.5c.09 3.58 1.16 4.5 4.99 4.5h10c4 0 5-1 5-5V9c0-4-1-5-5-5ZM8.993 4v3.5M8.993 16.5V20"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m15.025 9.33.62 1.25c.06.12.18.21.31.23l1.38.2c.34.05.48.47.23.71l-1 .97c-.1.09-.14.23-.12.37l.24 1.37c.06.34-.3.6-.6.44l-1.23-.65a.445.445 0 0 0-.39 0l-1.23.65c-.31.16-.66-.1-.6-.44l.24-1.37a.422.422 0 0 0-.12-.37l-.99-.97a.416.416 0 0 1 .23-.71l1.38-.2c.14-.02.25-.1.31-.23l.61-1.25c.14-.31.58-.31.73 0Z"
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
			d="M16.999 20.75h-10c-4.25 0-5.64-1.27-5.74-5.23 0-.2.07-.4.21-.54.14-.14.33-.23.54-.23 1.51 0 2.74-1.24 2.74-2.75s-1.23-2.75-2.74-2.75c-.2 0-.39-.08-.54-.23a.7.7 0 0 1-.21-.54c.1-3.96 1.49-5.23 5.74-5.23h10c4.41 0 5.75 1.34 5.75 5.75v6c0 4.41-1.34 5.75-5.75 5.75Zm-14.21-4.57c.17 2.54 1.03 3.07 4.21 3.07h10c3.58 0 4.25-.68 4.25-4.25V9c0-3.57-.67-4.25-4.25-4.25h-10c-3.18 0-4.04.54-4.21 3.07 1.97.38 3.46 2.11 3.46 4.18s-1.49 3.8-3.46 4.18Z"
			:fill="color"
		></path>
		<path
			d="M9 8.25c-.41 0-.75-.34-.75-.75V4c0-.41.34-.75.75-.75s.75.34.75.75v3.5c0 .41-.34.75-.75.75ZM9 20.75c-.41 0-.75-.34-.75-.75v-3.5c0-.41.34-.75.75-.75s.75.34.75.75V20c0 .41-.34.75-.75.75ZM13.04 15.652c-.24 0-.48-.08-.68-.22-.36-.26-.54-.7-.46-1.14l.21-1.19-.87-.85a1.17 1.17 0 0 1-.3-1.19c.14-.42.5-.73.94-.79l1.2-.18.54-1.09c.2-.4.6-.65 1.04-.65.45 0 .85.25 1.04.65l.54 1.09 1.2.18c.44.06.8.37.94.79.14.42.02.88-.3 1.19l-.87.85.21 1.19c.08.44-.1.88-.46 1.14-.36.26-.83.29-1.22.09l-1.07-.56-1.08.56c-.17.09-.36.13-.55.13Zm-.27-4 .51.5c.28.27.4.65.34 1.03l-.12.7.63-.33c.34-.18.74-.18 1.08 0l.63.33-.12-.7c-.06-.39.06-.77.34-1.03l.51-.5-.7-.1c-.38-.06-.71-.3-.88-.64l-.31-.64-.31.64c-.17.34-.5.58-.88.64l-.72.1Z"
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
			d="M16.994 4h-10c-3.83 0-4.9.92-4.99 4.5 1.93 0 3.49 1.57 3.49 3.5s-1.56 3.49-3.49 3.5c.09 3.58 1.16 4.5 4.99 4.5h10c4 0 5-1 5-5V9c0-4-1-5-5-5Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M8.992 4v3.5M8.992 16.5V20M15.024 9.33l.62 1.25c.06.12.18.21.31.23l1.38.2c.34.05.48.47.23.71l-1 .97c-.1.09-.14.23-.12.37l.24 1.37c.06.34-.3.6-.6.44l-1.23-.65a.445.445 0 0 0-.39 0l-1.23.65c-.31.16-.66-.1-.6-.44l.24-1.37a.422.422 0 0 0-.12-.37l-.99-.97a.416.416 0 0 1 .23-.71l1.38-.2c.14-.02.25-.1.31-.23l.61-1.25c.14-.31.58-.31.73 0Z"
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
	name: 'TicketStarIcon',
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
