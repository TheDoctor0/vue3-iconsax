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
			d="m20.049 10.629-4.67-2.01-1.04-.44a.585.585 0 0 1-.3-.47v-3.06c0-.96-.71-2.1-1.57-2.54-.3-.15-.66-.15-.96 0-.85.44-1.56 1.59-1.56 2.55v3.06c0 .18-.14.39-.3.47l-5.7 2.45c-.63.26-1.14 1.05-1.14 1.73v1.32c0 .85.64 1.27 1.43.93l5.01-2.16c.39-.17.71.04.71.47v2.91c0 .23-.13.56-.29.72l-2.32 2.33c-.24.24-.35.71-.24 1.05l.45 1.36c.18.59.85.87 1.4.59l2.38-2c.36-.31.95-.31 1.31 0l2.38 2c.55.27 1.22 0 1.42-.59l.45-1.36c.11-.33 0-.81-.24-1.05l-2.32-2.33c-.17-.16-.3-.49-.3-.72v-2.91c0-.43.31-.63.71-.47l5.01 2.16c.79.34 1.43-.08 1.43-.93v-1.32c0-.68-.51-1.47-1.14-1.74Z"
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
			d="m16.268 9.102-1.97-.85a.554.554 0 0 1-.3-.46v-3c0-.94-.69-2.05-1.53-2.48-.3-.15-.65-.15-.95 0-.84.43-1.53 1.55-1.53 2.49v3c0 .18-.14.39-.3.46l-5.58 2.41c-.62.25-1.12 1.02-1.12 1.69v1.29c0 .84.63 1.25 1.4.92l4.91-2.12c.38-.17.7.04.7.46v2.85c0 .23-.13.55-.29.71l-2.27 2.28c-.24.24-.35.7-.24 1.03l.44 1.33c.18.58.84.86 1.38.58l2.33-1.96c.35-.3.93-.3 1.28 0l2.33 1.96c.54.27 1.2 0 1.4-.58l.44-1.33c.11-.32 0-.79-.24-1.03l-2.27-2.28c-.17-.16-.3-.48-.3-.71v-2.85c0-.42.31-.62.7-.46l4.91 2.12c.77.33 1.4-.08 1.4-.92v-1.29c0-.67-.5-1.44-1.12-1.7"
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
			d="M9.959 14.039v-1.11c0-.43-.32-.64-.71-.47l-5.01 2.16c-.79.34-1.43-.08-1.43-.93v-1.32c0-.68.51-1.47 1.14-1.73l5.7-2.45c.16-.08.3-.29.3-.47v-3.06c0-.96.71-2.11 1.56-2.55.3-.15.66-.15.96 0 .86.44 1.57 1.58 1.57 2.54v3.06c0 .18.14.39.3.47l1.04.44-5.42 5.42Z"
			:fill="color"
		></path>
		<path
			opacity=".4"
			d="M21.19 12.371v1.32c0 .85-.64 1.27-1.43.93l-5.01-2.16c-.4-.16-.71.04-.71.47v2.91c0 .23.13.56.3.72l2.32 2.33c.24.24.35.72.24 1.05l-.45 1.36c-.2.59-.87.86-1.42.59l-2.38-2c-.36-.31-.95-.31-1.31 0l-2.38 2c-.55.28-1.22 0-1.4-.59l-.45-1.36c-.11-.34 0-.81.24-1.05l2.32-2.33c.16-.16.29-.49.29-.72v-1.8l5.42-5.42 4.67 2.01c.63.27 1.14 1.06 1.14 1.74Z"
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
			d="m9.03 21.69 2.33-1.96c.35-.3.93-.3 1.28 0l2.33 1.96c.54.27 1.2 0 1.4-.58l.44-1.33c.11-.32 0-.79-.24-1.03l-2.27-2.28c-.17-.16-.3-.48-.3-.71v-2.85c0-.42.31-.62.7-.46l4.91 2.12c.77.33 1.4-.08 1.4-.92v-1.29c0-.67-.5-1.44-1.12-1.7L14.3 8.25a.554.554 0 0 1-.3-.46v-3c0-.94-.69-2.05-1.53-2.48-.3-.15-.65-.15-.95 0-.84.43-1.53 1.55-1.53 2.49v3c0 .18-.14.39-.3.46l-5.58 2.41c-.62.25-1.12 1.02-1.12 1.69v1.29c0 .84.63 1.25 1.4.92l4.91-2.12c.38-.17.7.04.7.46v2.85c0 .23-.13.55-.29.71l-2.27 2.28c-.24.24-.35.7-.24 1.03l.44 1.33c.18.58.84.86 1.39.58Z"
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
			d="M8.582 22.55c-.22 0-.45-.04-.66-.13-.47-.2-.83-.59-.99-1.08l-.44-1.32c-.2-.6-.02-1.35.42-1.8l2.27-2.28c.03-.03.07-.14.07-.19v-2.47l-4.56 1.97c-.61.26-1.23.23-1.7-.08s-.75-.87-.75-1.52v-1.29c0-.98.7-2.03 1.59-2.38l5.41-2.34V4.8c0-1.21.85-2.6 1.93-3.16a1.8 1.8 0 0 1 1.63 0c1.09.56 1.94 1.94 1.94 3.15v2.84l5.44 2.34c.89.38 1.57 1.4 1.57 2.39v1.29c0 .66-.27 1.21-.75 1.52-.48.31-1.09.34-1.7.09l-4.56-1.97v2.47c0 .04.04.14.07.17l2.28 2.29c.44.44.62 1.21.42 1.8l-.44 1.32c-.17.49-.53.88-1.01 1.07-.47.19-.99.17-1.44-.05-.05-.03-.1-.06-.15-.1l-2.33-1.96c-.08-.07-.24-.06-.31 0l-2.33 1.96a.42.42 0 0 1-.14.09c-.24.14-.51.2-.78.2Zm.98-10.91c.23 0 .45.06.64.19.35.23.55.62.55 1.08v2.85c0 .43-.21.94-.51 1.24l-2.27 2.28c-.04.05-.08.2-.06.26l.44 1.33c.03.1.1.14.14.16.03.01.08.03.14.01l2.24-1.89c.63-.54 1.62-.54 2.25 0l2.23 1.88c.07.01.12 0 .15-.01.04-.02.12-.06.15-.16l.44-1.32a.376.376 0 0 0-.06-.26L13.762 17c-.3-.28-.52-.8-.52-1.24v-2.85c0-.45.19-.84.53-1.07.34-.23.78-.26 1.2-.08l4.92 2.12c.15.06.25.06.28.04.03-.02.07-.11.07-.27v-1.29c0-.38-.32-.87-.66-1.01l-5.58-2.41c-.44-.19-.75-.67-.75-1.15v-3c0-.66-.52-1.51-1.12-1.81a.319.319 0 0 0-.27 0c-.58.3-1.11 1.17-1.11 1.82v3c0 .47-.31.96-.75 1.15l-5.58 2.41c-.35.14-.67.63-.67 1v1.29c0 .16.04.25.07.27.03.02.13.02.28-.04l4.91-2.12c.18-.08.37-.12.55-.12Z"
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
			d="m9.028 21.692 2.33-1.96c.35-.3.93-.3 1.28 0l2.33 1.96c.54.27 1.2 0 1.4-.58l.44-1.33c.11-.32 0-.79-.24-1.03l-2.27-2.28c-.17-.16-.3-.48-.3-.71v-2.85c0-.42.31-.62.7-.46l4.91 2.12c.77.33 1.4-.08 1.4-.92v-1.29c0-.67-.5-1.44-1.12-1.7l-5.59-2.41a.554.554 0 0 1-.3-.46v-3c0-.94-.69-2.05-1.53-2.48-.3-.15-.65-.15-.95 0-.84.43-1.53 1.55-1.53 2.49v3c0 .18-.14.39-.3.46l-5.58 2.41c-.62.25-1.12 1.02-1.12 1.69v1.29c0 .84.63 1.25 1.4.92l4.91-2.12c.38-.17.7.04.7.46v2.85c0 .23-.13.55-.29.71l-2.27 2.28c-.24.24-.35.7-.24 1.03l.44 1.33c.18.58.84.86 1.39.58Z"
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
	name: 'AirplaneIcon',
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
