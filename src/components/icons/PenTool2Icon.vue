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
			d="M20.98 10.7a8.41 8.41 0 0 0-6.97-7.81c-.06-.77-.7-1.39-1.49-1.39h-1c-.79 0-1.42.61-1.49 1.38-3.88.64-6.79 3.9-7.01 7.82-.71.12-1.25.73-1.25 1.47v1c0 .83.67 1.5 1.5 1.5h1c.83 0 1.5-.67 1.5-1.5v-1c0-.74-.54-1.35-1.25-1.47a6.91 6.91 0 0 1 5.56-6.31c.17.64.75 1.11 1.44 1.11h1c.69 0 1.26-.47 1.44-1.1 3.04.61 5.31 3.2 5.52 6.3-.71.12-1.25.73-1.25 1.47v1c0 .83.67 1.5 1.5 1.5h1c.83 0 1.5-.67 1.5-1.5v-1c0-.74-.54-1.36-1.25-1.47Z"
			:fill="color"
		></path>
		<path
			d="M15.77 16.55 14.13 18H9.88l-1.64-1.45c-.95-.78-.95-1.38-.23-2.3l2.89-3.66c.2-.25.43-.42.69-.51.27-.09.56-.09.84 0 .25.09.48.26.69.51L16 14.24c.73.92.69 1.49-.23 2.31ZM13.32 22h-2.59c-.92 0-1.61-.75-1.43-1.55l.31-1.39a.6.6 0 0 1 .59-.47h3.65c.28 0 .52.19.59.47l.31 1.39c.19.85-.45 1.55-1.43 1.55Z"
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
			d="M10.751 22.503h2.52c.96 0 1.58-.68 1.4-1.51l-.41-1.81h-4.5l-.41 1.81c-.18.78.5 1.51 1.4 1.51ZM14.22 12.672l-1.05-1.33c-.64-.81-1.69-.81-2.33 0l-3.05 3.87c-.77.97-.77 1.6.24 2.43l1.73 1.54M14.262 19.173l1.73-1.54c.97-.86 1.01-1.46.24-2.43M12.012 11.121v2.53M12.52 5h-1c-.55 0-1-.45-1-1V3c0-.55.45-1 1-1h1c.55 0 1 .45 1 1v1c0 .55-.45 1-1 1ZM3.27 14.172h1c.55 0 1-.45 1-1v-1c0-.55-.45-1-1-1h-1c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1ZM20.73 14.172h-1c-.55 0-1-.45-1-1v-1c0-.55.45-1 1-1h1c.55 0 1 .45 1 1v1c0 .55-.45 1-1 1ZM3.75 11.17c0-1.97.74-3.76 1.96-5.12M10.52 3.559a8.2 8.2 0 0 0-1.85.45"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M20.25 11.169c0-3.92-2.94-7.14-6.73-7.61"
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
			d="M12.52 1.5h-1c-.83 0-1.5.67-1.5 1.5v1c0 .83.67 1.5 1.5 1.5h1c.83 0 1.5-.67 1.5-1.5V3c0-.83-.67-1.5-1.5-1.5ZM4.27 10.672h-1c-.83 0-1.5.67-1.5 1.5v1c0 .83.67 1.5 1.5 1.5h1c.83 0 1.5-.67 1.5-1.5v-1c0-.83-.68-1.5-1.5-1.5ZM20.73 10.672h-1c-.83 0-1.5.67-1.5 1.5v1c0 .83.67 1.5 1.5 1.5h1c.83 0 1.5-.67 1.5-1.5v-1c0-.83-.67-1.5-1.5-1.5Z"
			:fill="color"
		></path>
		<path
			d="M3.75 11.918c-.41 0-.75-.34-.75-.75 0-4.27 3.2-7.86 7.44-8.36.4-.04.78.25.83.66.05.41-.25.78-.66.83a6.92 6.92 0 0 0-6.11 6.87c0 .41-.34.75-.75.75ZM20.249 11.92c-.41 0-.75-.34-.75-.75 0-3.49-2.61-6.44-6.07-6.86a.744.744 0 0 1-.65-.83c.05-.41.43-.7.84-.65 4.21.51 7.39 4.1 7.39 8.35-.01.4-.34.74-.76.74ZM13.29 22.007h-2.57c-.92 0-1.6-.74-1.43-1.54l.42-1.85h4.59l.42 1.85c.19.85-.45 1.54-1.43 1.54Z"
			:fill="color"
		></path>
		<path
			opacity=".4"
			d="m16.07 17.049-1.77 1.57H9.71l-1.77-1.57c-1.03-.84-1.03-1.49-.25-2.48l3.12-3.94c.22-.27.47-.46.74-.55.29-.1.61-.1.9 0 .27.1.52.28.74.55l3.12 3.94c.78.99.75 1.61-.24 2.48Z"
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
			:stroke="color"
			stroke-linecap="round"
			stroke-linejoin="round"
			:stroke-width="strokeWidth"
			d="M10.75 22.5h2.52c.96 0 1.58-.68 1.4-1.51l-.41-1.81h-4.5l-.41 1.81c-.18.78.5 1.51 1.4 1.51zM14.26 19.17l1.73-1.54c.97-.86 1.01-1.46.24-2.43l-3.05-3.87c-.64-.81-1.69-.81-2.33 0L7.8 15.2c-.77.97-.77 1.6.24 2.43l1.73 1.54M12.01 11.12v2.53"
		></path>
		<g>
			<path
				:stroke="color"
				stroke-linecap="round"
				stroke-linejoin="round"
				:stroke-width="strokeWidth"
				d="M12.52 5h-1c-.55 0-1-.45-1-1V3c0-.55.45-1 1-1h1c.55 0 1 .45 1 1v1c0 .55-.45 1-1 1zM3.27 14.17h1c.55 0 1-.45 1-1v-1c0-.55-.45-1-1-1h-1c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1zM20.73 14.17h-1c-.55 0-1-.45-1-1v-1c0-.55.45-1 1-1h1c.55 0 1 .45 1 1v1c0 .55-.45 1-1 1zM10.52 3.56c-3.81.45-6.77 3.68-6.77 7.61M20.25 11.17c0-3.92-2.94-7.14-6.73-7.61"
			></path>
		</g>
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
			d="M13.27 23.252h-2.52c-.7 0-1.33-.3-1.75-.81-.37-.46-.51-1.05-.38-1.61l.41-1.81c.08-.34.38-.58.73-.58h4.5c.35 0 .65.24.73.58l.41 1.81c.13.6.01 1.18-.36 1.64-.41.49-1.05.78-1.77.78Zm-2.91-3.33-.28 1.23a.4.4 0 0 0 .09.34c.13.16.34.25.58.25h2.52c.26 0 .48-.08.6-.23.08-.1.1-.22.07-.37l-.28-1.23h-3.3v.01Z"
			:fill="color"
		></path>
		<path
			d="M14.26 19.919c-.21 0-.41-.08-.56-.25a.756.756 0 0 1 .06-1.06l1.73-1.54c.69-.61.66-.76.15-1.4l-3.05-3.87c-.17-.21-.37-.33-.58-.33-.21 0-.41.12-.58.33l-3.05 3.87c-.54.69-.53.84.13 1.38l1.75 1.56c.31.27.34.75.06 1.06-.28.31-.75.34-1.06.06l-1.73-1.54c-1.26-1.03-1.37-2.13-.33-3.45l3.05-3.87c.45-.57 1.09-.9 1.76-.9.67 0 1.31.33 1.76.9l3.05 3.87c1.03 1.3.93 2.34-.33 3.45l-1.73 1.54c-.15.13-.33.19-.5.19Z"
			:fill="color"
		></path>
		<path
			d="M12.01 14.401c-.41 0-.75-.34-.75-.75v-2.53c0-.41.34-.75.75-.75s.75.34.75.75v2.53c0 .42-.34.75-.75.75ZM12.52 5.75h-1c-.96 0-1.75-.79-1.75-1.75V3c0-.96.79-1.75 1.75-1.75h1c.96 0 1.75.79 1.75 1.75v1c0 .96-.78 1.75-1.75 1.75Zm-1-3c-.14 0-.25.11-.25.25v1c0 .14.11.25.25.25h1c.14 0 .25-.11.25-.25V3c0-.14-.11-.25-.25-.25h-1ZM4.27 14.922h-1c-.96 0-1.75-.79-1.75-1.75v-1c0-.96.79-1.75 1.75-1.75h1c.96 0 1.75.79 1.75 1.75v1c0 .96-.79 1.75-1.75 1.75Zm-1-3c-.14 0-.25.11-.25.25v1c0 .14.11.25.25.25h1c.14 0 .25-.11.25-.25v-1c0-.14-.11-.25-.25-.25h-1ZM20.73 14.922h-1c-.96 0-1.75-.79-1.75-1.75v-1c0-.96.79-1.75 1.75-1.75h1c.96 0 1.75.79 1.75 1.75v1c0 .96-.78 1.75-1.75 1.75Zm-1-3c-.14 0-.25.11-.25.25v1c0 .14.11.25.25.25h1c.14 0 .25-.11.25-.25v-1c0-.14-.11-.25-.25-.25h-1Z"
			:fill="color"
		></path>
		<path
			d="M3.75 11.918c-.41 0-.75-.34-.75-.75 0-4.27 3.2-7.86 7.44-8.36.41-.04.78.25.83.66.05.41-.25.78-.66.83a6.92 6.92 0 0 0-6.11 6.87c0 .41-.34.75-.75.75ZM20.249 11.922c-.41 0-.75-.34-.75-.75 0-3.49-2.61-6.44-6.07-6.86a.744.744 0 0 1-.65-.83.74.74 0 0 1 .84-.65c4.21.51 7.39 4.1 7.39 8.35-.01.4-.34.74-.76.74Z"
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
			<path
				d="M10.75 22.5h2.52c.96 0 1.58-.68 1.4-1.51l-.41-1.81h-4.5l-.41 1.81c-.18.78.5 1.51 1.4 1.51ZM14.26 19.17l1.73-1.54c.97-.86 1.01-1.46.24-2.43l-3.05-3.87c-.64-.81-1.69-.81-2.33 0L7.8 15.2c-.77.97-.77 1.6.24 2.43l1.73 1.54M12.01 11.121v2.53"
			></path>
		</g>
		<path
			d="M12.52 5h-1c-.55 0-1-.45-1-1V3c0-.55.45-1 1-1h1c.55 0 1 .45 1 1v1c0 .55-.45 1-1 1ZM3.27 14.172h1c.55 0 1-.45 1-1v-1c0-.55-.45-1-1-1h-1c-.55 0-1 .45-1 1v1c0 .55.45 1 1 1ZM20.73 14.172h-1c-.55 0-1-.45-1-1v-1c0-.55.45-1 1-1h1c.55 0 1 .45 1 1v1c0 .55-.45 1-1 1ZM10.52 3.559c-3.81.45-6.77 3.68-6.77 7.61M20.25 11.169c0-3.92-2.94-7.14-6.73-7.61"
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
	name: 'PenTool2Icon',
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
