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
			d="m20.86 8.561-6.93-5.54c-1.07-.86-2.8-.86-3.86-.01l-6.93 5.55c-.78.62-1.28 1.93-1.11 2.91l1.33 7.96c.24 1.42 1.6 2.57 3.04 2.57h11.2c1.43 0 2.8-1.16 3.04-2.57l1.33-7.96c.16-.98-.34-2.29-1.11-2.91Zm-11.48 8.82c-.56 0-1-.45-1-1s.45-1 1-1 1 .45 1 1-.45 1-1 1Zm3.01-.26h-.02c-.41 0-.74-.33-.75-.73-.03-1.35-.92-2.24-2.27-2.27a.75.75 0 0 1-.73-.77c.01-.41.34-.73.75-.73h.02c2.15.05 3.69 1.58 3.73 3.73.01.42-.31.77-.73.77Zm2.99 0c-.42 0-.75-.33-.76-.74-.01-.66-.12-1.29-.32-1.88-.51-1.46-1.6-2.54-3.06-3.06-.59-.21-1.22-.32-1.88-.32-.41 0-.75-.34-.74-.76 0-.41.34-.74.75-.74h.01c.83.01 1.62.15 2.36.41 1.89.67 3.3 2.08 3.97 3.97.26.74.4 1.54.41 2.36.01.42-.32.76-.74.76Z"
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
			d="M21.97 11.28c.16-.98-.34-2.29-1.11-2.91l-6.93-5.54c-1.07-.86-2.8-.86-3.86-.01L3.14 8.37c-.78.62-1.28 1.93-1.11 2.91l.28 1.68M11.4 21.81h6.2c1.43 0 2.8-1.16 3.04-2.57l.63-3.74M2 19c1.76.04 2.96 1.24 3 3M2 16c.52.01 1.02.07 1.5.18M8 22c-.01-.76-.14-1.47-.37-2.12-.27-.76-.67-1.43-1.19-1.99"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M1.996 22h.009"
			:stroke="color"
			stroke-width="2"
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
			d="m10.07 3.011-6.93 5.55c-.78.62-1.28 1.93-1.11 2.91l1.33 7.96c.24 1.42 1.6 2.57 3.04 2.57h11.2c1.43 0 2.8-1.16 3.04-2.57l1.33-7.96c.16-.98-.34-2.29-1.11-2.91l-6.93-5.54c-1.07-.86-2.8-.86-3.86-.01Z"
			:fill="color"
		></path>
		<path
			d="M12.371 17.121c-.41 0-.74-.33-.75-.73-.03-1.35-.92-2.24-2.27-2.27a.75.75 0 0 1-.73-.77c.01-.41.34-.73.75-.73h.02c2.15.05 3.69 1.58 3.73 3.73.01.41-.32.76-.73.77h-.02Z"
			:fill="color"
		></path>
		<path
			d="M15.371 17.121c-.41 0-.75-.33-.75-.74-.01-.66-.12-1.29-.32-1.88-.51-1.46-1.6-2.54-3.06-3.06-.59-.21-1.22-.32-1.88-.32-.41 0-.75-.34-.74-.76 0-.41.34-.74.75-.74h.01c.83.01 1.62.15 2.36.41 1.89.67 3.3 2.08 3.97 3.97.26.74.4 1.54.41 2.36.01.42-.32.76-.75.76.01 0 .01 0 0 0ZM9.38 17.383c-.56 0-1-.45-1-1s.45-1 1-1 1 .45 1 1-.45 1-1 1Z"
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
			d="M11.4 21.81h6.2c1.43 0 2.8-1.16 3.04-2.57l1.33-7.96c.16-.98-.34-2.29-1.11-2.91l-6.93-5.54c-1.07-.86-2.8-.86-3.86-.01L3.14 8.37c-.78.62-1.28 1.93-1.11 2.91l.28 1.68M2 19c1.76.04 2.96 1.24 3 3M8 22c-.01-.76-.14-1.47-.37-2.12a5.688 5.688 0 0 0-3.51-3.51c-.65-.23-1.36-.36-2.12-.37"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M1.996 22h.009"
			:stroke="color"
			stroke-width="2"
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
			d="M17.6 22.56h-6.2c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h6.2c1.07 0 2.12-.89 2.3-1.95l1.33-7.96c.12-.72-.28-1.75-.84-2.2l-6.93-5.54c-.8-.64-2.13-.64-2.92-.01L3.61 8.95c-.57.46-.96 1.48-.84 2.2l.28 1.69c.07.41-.21.8-.62.86-.41.08-.79-.21-.86-.62l-.28-1.68c-.21-1.24.39-2.83 1.38-3.62L9.6 2.23c1.34-1.08 3.45-1.07 4.8.01l6.93 5.54c.98.79 1.58 2.38 1.38 3.62l-1.33 7.96c-.3 1.77-1.99 3.2-3.78 3.2ZM5 22.75c-.41 0-.74-.33-.75-.73-.03-1.35-.92-2.24-2.27-2.27a.75.75 0 0 1-.73-.77c.01-.41.34-.73.75-.73h.02c2.15.05 3.69 1.58 3.73 3.73.01.41-.32.76-.73.77H5Z"
			:fill="color"
		></path>
		<path
			d="M8 22.75c-.41 0-.75-.33-.75-.74-.01-.66-.12-1.29-.32-1.88-.51-1.46-1.6-2.54-3.06-3.06-.59-.21-1.22-.32-1.88-.32-.41 0-.75-.34-.74-.76 0-.41.34-.74.75-.74h.01c.83.01 1.62.15 2.36.41 1.89.67 3.3 2.08 3.97 3.97.26.74.4 1.54.41 2.36 0 .42-.33.76-.75.76 0 0 .01 0 0 0ZM2 23c-.56 0-1-.45-1-1s.45-1 1-1 1 .45 1 1-.44 1-1 1Z"
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
			d="M11.4 21.81h6.2c1.43 0 2.8-1.16 3.04-2.57l1.33-7.96c.16-.98-.34-2.29-1.11-2.91l-6.93-5.54c-1.07-.86-2.8-.86-3.86-.01L3.14 8.37c-.78.62-1.28 1.93-1.11 2.91l.28 1.68"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M2 19c1.76.04 2.96 1.24 3 3M8 22c-.01-.76-.14-1.47-.37-2.12a5.688 5.688 0 0 0-3.51-3.51c-.65-.23-1.36-.36-2.12-.37"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M1.996 22h.009"
			:stroke="color"
			stroke-width="2"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
	</svg>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
	name: 'SmartHomeIcon',
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
