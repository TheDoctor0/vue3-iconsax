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
			d="M3.23 1h8.13c.68 0 1.23.56 1.23 1.25v1.37c0 .5-.31 1.12-.62 1.43L9.33 7.43c-.37.31-.61.93-.61 1.43v2.68c0 .37-.25.87-.55 1.06l-.87.57c-.8.5-1.91-.06-1.91-1.06V8.8c0-.44-.25-1-.49-1.31l-2.34-2.5C2.25 4.68 2 4.12 2 3.75V2.31C2 1.56 2.55 1 3.23 1Z"
			:fill="color"
		></path>
		<path
			d="M17 2h-2.4c-.28 0-.5.22-.5.5v1.12c0 .99-.53 1.96-1.05 2.49l-2.72 2.43c-.03.07-.08.17-.11.25v2.75c0 .91-.54 1.9-1.28 2.35l-.82.53c-.46.29-.97.43-1.48.43-.46 0-.92-.12-1.34-.35a2.718 2.718 0 0 1-1.147-1.226c-.122-.26-.153-.55-.153-.836V10.21a.47.47 0 0 0-.15-.35l-1-1a.495.495 0 0 0-.85.35V17c0 2.76 2.24 5 5 5h10c2.76 0 5-2.24 5-5V7c0-2.76-2.24-5-5-5Zm1 15.75h-7c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h7c.41 0 .75.34.75.75s-.34.75-.75.75Zm0-4h-5c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h5c.41 0 .75.34.75.75s-.34.75-.75.75Z"
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
			d="M3.35 2h8.9c.74 0 1.35.61 1.35 1.35v1.48c0 .54-.34 1.21-.67 1.55l-2.9 2.56c-.4.34-.67 1.01-.67 1.55v2.9c0 .4-.27.94-.61 1.15l-.94.61c-.88.54-2.09-.07-2.09-1.15v-3.57c0-.47-.27-1.08-.54-1.42l-2.56-2.7c-.34-.34-.61-.94-.61-1.35V3.41C2 2.61 2.61 2 3.35 2Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22 8.998c0-3.12-.78-5.08-2.59-6.1-.51-.29-1.53-.51-2.46-.66M2 12v3c0 5 2 7 7 7h6c5 0 7-2 7-7v-2M13 13h5M11 17h7"
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
			d="M3.23 1h8.13c.68 0 1.23.56 1.23 1.25v1.37c0 .5-.31 1.12-.62 1.43L9.32 7.42c-.37.31-.62.94-.62 1.43v2.68c0 .37-.25.87-.55 1.06l-.86.56c-.8.5-1.91-.06-1.91-1.06V8.78c0-.44-.25-1-.49-1.31l-2.34-2.5C2.24 4.66 2 4.1 2 3.72V2.29C2 1.56 2.55 1 3.23 1Z"
			:fill="color"
		></path>
		<path
			opacity=".4"
			d="M17 2h-2.4c-.28 0-.5.22-.5.5v1.12c0 .99-.53 1.96-1.05 2.49l-2.72 2.43c-.03.07-.08.17-.11.25v2.75c0 .91-.54 1.9-1.28 2.35l-.82.53c-.46.29-.97.43-1.48.43-.46 0-.92-.12-1.34-.35-.65-.36-1.1-.95-1.3-1.63v-2.66a.47.47 0 0 0-.15-.35l-1-1c-.32-.31-.85-.09-.85.35V17c0 2.76 2.24 5 5 5h10c2.76 0 5-2.24 5-5V7c0-2.76-2.24-5-5-5Z"
			:fill="color"
		></path>
		<path
			d="M18 13.75h-5c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h5c.41 0 .75.34.75.75s-.34.75-.75.75ZM18 17.75h-7c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h7c.41 0 .75.34.75.75s-.34.75-.75.75Z"
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
			d="M3.35 2h8.9c.74 0 1.35.61 1.35 1.35v1.48c0 .54-.34 1.21-.67 1.55l-2.9 2.56c-.4.34-.67 1.01-.67 1.55v2.9c0 .4-.27.94-.61 1.15l-.94.61c-.88.54-2.09-.07-2.09-1.15v-3.57c0-.47-.27-1.08-.54-1.42l-2.56-2.7c-.34-.34-.61-.94-.61-1.35V3.41C2 2.61 2.61 2 3.35 2Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M2 12v3c0 5 2 7 7 7h6c5 0 7-2 7-7V9c0-3.12-.78-5.08-2.59-6.1-.51-.29-1.53-.51-2.46-.66M13 13h5M11 17h7"
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
			d="M7.08 16.098c-.36 0-.72-.09-1.05-.28a2.074 2.074 0 0 1-1.07-1.82v-3.57c0-.26-.17-.7-.38-.95l-2.52-2.65c-.47-.46-.81-1.26-.81-1.87v-1.55c0-1.21.92-2.17 2.1-2.17h8.9c1.16 0 2.1.94 2.1 2.1v1.48c0 .78-.45 1.64-.89 2.08l-2.93 2.59c-.23.19-.42.65-.42.99v2.9c0 .69-.42 1.46-.97 1.79l-.92.6c-.36.22-.75.33-1.14.33ZM3.35 2.748c-.34 0-.6.29-.6.67v1.55c0 .17.17.6.39.82l2.58 2.71c.38.47.75 1.24.75 1.93v3.57c0 .3.19.45.31.51.16.09.42.14.64 0l.93-.6c.12-.07.26-.35.26-.52v-2.9c0-.79.39-1.66.94-2.13l2.88-2.55c.18-.18.42-.67.42-.99v-1.48c0-.33-.27-.6-.6-.6h-8.9v.01Z"
			:fill="color"
		></path>
		<path
			d="M15 22.749H9c-5.43 0-7.75-2.32-7.75-7.75v-3c0-.41.34-.75.75-.75s.75.34.75.75v3c0 4.61 1.64 6.25 6.25 6.25h6c4.61 0 6.25-1.64 6.25-6.25v-6c0-2.9-.68-4.58-2.21-5.45-.16-.09-.69-.33-2.21-.57a.742.742 0 0 1-.62-.86c.07-.41.46-.69.86-.62 1.31.21 2.2.45 2.71.74 2.02 1.15 2.97 3.3 2.97 6.76v6c0 5.43-2.32 7.75-7.75 7.75Z"
			:fill="color"
		></path>
		<path
			d="M18 13.75h-5c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h5c.41 0 .75.34.75.75s-.34.75-.75.75ZM18 17.75h-7c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h7c.41 0 .75.34.75.75s-.34.75-.75.75Z"
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
			d="M3.35 2h8.9c.74 0 1.35.61 1.35 1.35v1.48c0 .54-.34 1.21-.67 1.55l-2.9 2.56c-.4.34-.67 1.01-.67 1.55v2.9c0 .4-.27.94-.61 1.15l-.94.61c-.88.54-2.09-.07-2.09-1.15v-3.57c0-.47-.27-1.08-.54-1.42l-2.56-2.7c-.34-.34-.61-.94-.61-1.35V3.41C2 2.61 2.61 2 3.35 2Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M2 11.998v3c0 5 2 7 7 7h6c5 0 7-2 7-7v-6c0-3.12-.78-5.08-2.59-6.1-.51-.29-1.53-.51-2.46-.66"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M13 13h5M11 17h7"
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
	name: 'DocumentFilterIcon',
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
