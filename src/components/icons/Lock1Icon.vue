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
			d="M18.75 8v2.1c-.44-.06-.94-.09-1.5-.1V8c0-3.15-.89-5.25-5.25-5.25S6.75 4.85 6.75 8v2c-.56.01-1.06.04-1.5.1V8c0-2.9.7-6.75 6.75-6.75S18.75 5.1 18.75 8Z"
			:fill="color"
		></path>
		<path
			d="M18.75 10.1c-.44-.06-.94-.09-1.5-.1H6.75c-.56.01-1.06.04-1.5.1C2.7 10.41 2 11.66 2 15v2c0 4 1 5 5 5h10c4 0 5-1 5-5v-2c0-3.34-.7-4.59-3.25-4.9ZM8.71 16.71c-.19.18-.45.29-.71.29-.13 0-.26-.03-.38-.08-.13-.05-.23-.12-.33-.21-.18-.19-.29-.45-.29-.71 0-.13.03-.26.08-.38s.12-.23.21-.33c.1-.09.2-.16.33-.21.37-.16.81-.07 1.09.21.09.1.16.21.21.33.05.12.08.25.08.38 0 .26-.11.52-.29.71Zm4.21-.33c-.05.12-.12.23-.21.33-.19.18-.45.29-.71.29-.27 0-.52-.11-.71-.29-.09-.1-.16-.21-.21-.33A.995.995 0 0 1 11 16c0-.27.11-.52.29-.71.37-.37 1.04-.37 1.42 0 .18.19.29.44.29.71 0 .13-.03.26-.08.38Zm3.79.33c-.19.18-.45.29-.71.29-.26 0-.52-.11-.71-.29-.18-.19-.29-.44-.29-.71 0-.27.11-.52.29-.71.38-.37 1.05-.37 1.42 0 .04.05.08.1.12.16.04.05.07.11.09.17.03.06.05.12.06.18.01.07.02.14.02.2 0 .26-.11.52-.29.71Z"
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
			d="M6 10V8c0-3.31 1-6 6-6s6 2.69 6 6v2M9.5 16a2.5 2.5 0 0 0 5 0 2.5 2.5 0 0 0-2.5-2.5"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 17v-2c0-4-1-5-5-5H7c-4 0-5 1-5 5v2c0 4 1 5 5 5h10c1.76 0 2.94-.19 3.71-.75"
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
			d="M12.001 17.35a1.63 1.63 0 1 0 0-3.26 1.63 1.63 0 0 0 0 3.26Z"
			:fill="color"
		></path>
		<path
			d="M16.65 9.441h-9.3c-4.1 0-5.35 1.25-5.35 5.35v1.86c0 4.1 1.25 5.35 5.35 5.35h9.3c4.1 0 5.35-1.25 5.35-5.35v-1.86c0-4.1-1.25-5.35-5.35-5.35Zm-4.65 9.3c-1.67 0-3.02-1.36-3.02-3.02s1.35-3.02 3.02-3.02 3.02 1.36 3.02 3.02-1.35 3.02-3.02 3.02Z"
			:fill="color"
		></path>
		<path
			opacity=".4"
			d="M7.119 9.45V8.28c0-2.93.83-4.88 4.88-4.88s4.88 1.95 4.88 4.88v1.17c.51.01.97.03 1.4.09V8.28c0-2.7-.65-6.28-6.28-6.28s-6.28 3.58-6.28 6.28v1.25c.42-.05.89-.08 1.4-.08Z"
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
			d="M6 10V8c0-3.31 1-6 6-6s6 2.69 6 6v2M12 18.5a2.5 2.5 0 1 0 0-5 2.5 2.5 0 0 0 0 5Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M17 22H7c-4 0-5-1-5-5v-2c0-4 1-5 5-5h10c4 0 5 1 5 5v2c0 4-1 5-5 5Z"
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
			d="M18 10.75c-.41 0-.75-.34-.75-.75V8c0-3.15-.89-5.25-5.25-5.25S6.75 4.85 6.75 8v2c0 .41-.34.75-.75.75s-.75-.34-.75-.75V8c0-2.9.7-6.75 6.75-6.75S18.75 5.1 18.75 8v2c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M17 22.75H7c-4.41 0-5.75-1.34-5.75-5.75v-2c0-4.41 1.34-5.75 5.75-5.75h10c4.41 0 5.75 1.34 5.75 5.75v2c0 4.41-1.34 5.75-5.75 5.75Zm-10-12c-3.58 0-4.25.68-4.25 4.25v2c0 3.57.67 4.25 4.25 4.25h10c3.58 0 4.25-.68 4.25-4.25v-2c0-3.57-.67-4.25-4.25-4.25H7Z"
			:fill="color"
		></path>
		<path
			d="M8 16.999c-.13 0-.26-.03-.38-.08-.13-.05-.23-.12-.33-.21-.18-.19-.29-.44-.29-.71 0-.13.03-.26.08-.38.05-.13.12-.23.21-.33.1-.09.2-.16.33-.21.36-.16.81-.07 1.09.21.09.1.16.21.21.33.05.12.08.25.08.38 0 .26-.11.52-.29.71-.19.18-.45.29-.71.29ZM12 17c-.26 0-.52-.11-.71-.29-.18-.19-.29-.44-.29-.71 0-.13.02-.26.08-.38.05-.12.12-.23.21-.33.23-.23.58-.34.9-.27.07.01.13.03.19.06.06.02.12.05.18.09.05.03.1.08.15.12.09.1.16.21.21.33.05.12.08.25.08.38 0 .27-.11.52-.29.71l-.15.12c-.06.04-.12.07-.18.09-.06.03-.12.05-.19.06-.06.01-.13.02-.19.02ZM16 17c-.27 0-.52-.11-.71-.29-.09-.1-.16-.21-.21-.33A.995.995 0 0 1 15 16c0-.26.11-.52.29-.71l.15-.12c.06-.04.12-.07.18-.09.06-.03.12-.05.18-.06.33-.07.67.04.91.27.18.19.29.44.29.71 0 .13-.03.26-.08.38-.05.13-.12.23-.21.33-.19.18-.45.29-.71.29Z"
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
			d="M6 10V8c0-3.31 1-6 6-6s6 2.69 6 6v2M12 18.5a2.5 2.5 0 1 0 0-5 2.5 2.5 0 0 0 0 5Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M17 22H7c-4 0-5-1-5-5v-2c0-4 1-5 5-5h10c4 0 5 1 5 5v2c0 4-1 5-5 5Z"
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
	name: 'Lock1Icon',
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
