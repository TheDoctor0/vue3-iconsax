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
			d="M22 9.75c-.41 0-.75-.34-.75-.75V7c0-2.58-1.67-4.25-4.25-4.25H7C4.42 2.75 2.75 4.42 2.75 7v2c0 .41-.34.75-.75.75s-.75-.34-.75-.75V7c0-3.44 2.31-5.75 5.75-5.75h10c3.44 0 5.75 2.31 5.75 5.75v2c0 .41-.34.75-.75.75ZM17 22.75H7c-3.44 0-5.75-2.31-5.75-5.75v-2c0-.41.34-.75.75-.75s.75.34.75.75v2c0 2.58 1.67 4.25 4.25 4.25h10c2.58 0 4.25-1.67 4.25-4.25v-2c0-.41.34-.75.75-.75s.75.34.75.75v2c0 3.44-2.31 5.75-5.75 5.75Z"
			:fill="color"
		></path>
		<path
			d="m16.4 8.21-3.76-2.03c-.4-.21-.87-.21-1.27 0L7.6 8.21c-.27.15-.44.44-.44.76 0 .33.17.62.44.77l3.76 2.03c.2.11.42.16.64.16.22 0 .44-.05.64-.16l3.76-2.03a.87.87 0 0 0 .44-.77c0-.32-.17-.61-.44-.76ZM10.74 12.469l-3.5-1.75a.867.867 0 0 0-.84.04.86.86 0 0 0-.4.73v3.31c0 .57.32 1.09.83 1.34l3.5 1.75c.12.06.25.09.39.09.16 0 .31-.04.45-.13.26-.16.41-.43.41-.73v-3.31c-.01-.57-.32-1.08-.84-1.34ZM17.592 10.758a.867.867 0 0 0-.84-.04l-3.5 1.75a1.5 1.5 0 0 0-.83 1.34v3.31c0 .3.15.57.41.73.14.09.29.13.45.13.13 0 .26-.03.39-.09l3.5-1.75c.51-.26.83-.77.83-1.34v-3.31c0-.3-.15-.57-.41-.73Z"
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
			d="M17 2c3 0 5 2 5 5v2M2 9V7c0-3 2-5 5-5h5.77M21.999 15v2c0 3-2 5-5 5h-5.53M2 15v2c0 3 2 5 5 5"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m6.7 9.262 5.3 3.07 5.26-3.05M12 17.77v-5.45"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m10.758 6.289-3.2 1.78c-.72.4-1.32 1.41-1.32 2.24v3.39c0 .83.59 1.84 1.32 2.24l3.2 1.78c.68.38 1.8.38 2.49 0l3.2-1.78c.72-.4 1.32-1.41 1.32-2.24v-3.39c0-.83-.59-1.84-1.32-2.24l-3.2-1.78c-.69-.39-1.81-.39-2.49 0Z"
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
			d="M22 9.75c-.41 0-.75-.34-.75-.75V7c0-2.58-1.67-4.25-4.25-4.25H7C4.42 2.75 2.75 4.42 2.75 7v2c0 .41-.34.75-.75.75s-.75-.34-.75-.75V7c0-3.44 2.31-5.75 5.75-5.75h10c3.44 0 5.75 2.31 5.75 5.75v2c0 .41-.34.75-.75.75ZM17 22.75H7c-3.44 0-5.75-2.31-5.75-5.75v-2c0-.41.34-.75.75-.75s.75.34.75.75v2c0 2.58 1.67 4.25 4.25 4.25h10c2.58 0 4.25-1.67 4.25-4.25v-2c0-.41.34-.75.75-.75s.75.34.75.75v2c0 3.44-2.31 5.75-5.75 5.75Z"
			:fill="color"
		></path>
		<path
			d="m16.402 8.211-3.76-2.03c-.4-.21-.87-.21-1.27 0l-3.76 2.03a.87.87 0 0 0-.44.77c0 .33.17.62.44.77l3.76 2.03c.2.11.42.16.64.16.22 0 .44-.05.64-.16l3.76-2.03a.87.87 0 0 0 .44-.77.9.9 0 0 0-.45-.77ZM10.738 12.468l-3.5-1.75a.867.867 0 0 0-.84.04c-.26.16-.41.43-.41.73v3.31c0 .57.32 1.09.83 1.34l3.5 1.75c.12.06.25.09.39.09.16 0 .31-.04.45-.13.26-.16.41-.43.41-.73v-3.31c0-.57-.31-1.08-.83-1.34ZM17.592 10.758a.867.867 0 0 0-.84-.04l-3.5 1.75a1.5 1.5 0 0 0-.83 1.34v3.31c0 .3.15.57.41.73.14.09.29.13.45.13.13 0 .26-.03.39-.09l3.5-1.75c.51-.26.83-.77.83-1.34v-3.31c0-.3-.15-.57-.41-.73Z"
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
			d="M2 9V7c0-3 2-5 5-5h10c3 0 5 2 5 5v2M2 15v2c0 3 2 5 5 5h10c3 0 5-2 5-5v-2"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m6.7 9.26 5.3 3.07 5.26-3.05M12 17.77v-5.45"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m10.76 6.29-3.2 1.78c-.72.4-1.32 1.41-1.32 2.24v3.39c0 .83.59 1.84 1.32 2.24l3.2 1.78c.68.38 1.8.38 2.49 0l3.2-1.78c.72-.4 1.32-1.41 1.32-2.24v-3.39c0-.83-.59-1.84-1.32-2.24l-3.2-1.78c-.69-.39-1.81-.39-2.49 0Z"
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
			d="M22 9.75c-.41 0-.75-.34-.75-.75V7c0-2.58-1.67-4.25-4.25-4.25H7C4.42 2.75 2.75 4.42 2.75 7v2c0 .41-.34.75-.75.75s-.75-.34-.75-.75V7c0-3.44 2.31-5.75 5.75-5.75h10c3.44 0 5.75 2.31 5.75 5.75v2c0 .41-.34.75-.75.75ZM17 22.75H7c-3.44 0-5.75-2.31-5.75-5.75v-2c0-.41.34-.75.75-.75s.75.34.75.75v2c0 2.58 1.67 4.25 4.25 4.25h10c2.58 0 4.25-1.67 4.25-4.25v-2c0-.41.34-.75.75-.75s.75.34.75.75v2c0 3.44-2.31 5.75-5.75 5.75Z"
			:fill="color"
		></path>
		<path
			d="M11.999 13.079c-.13 0-.26-.03-.38-.1l-5.3-3.06a.752.752 0 0 1-.27-1.03c.21-.36.67-.48 1.02-.27l4.92 2.85 4.89-2.83c.36-.21.82-.08 1.02.27.21.36.08.82-.27 1.03l-5.26 3.04c-.11.06-.24.1-.37.1Z"
			:fill="color"
		></path>
		<path
			d="M12 18.518c-.41 0-.75-.34-.75-.75v-5.44c0-.41.34-.75.75-.75s.75.34.75.75v5.44c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M12.002 18.75c-.58 0-1.15-.13-1.61-.38l-3.2-1.78c-.96-.53-1.7-1.8-1.7-2.9V10.3c0-1.09.75-2.36 1.7-2.9l3.2-1.78c.92-.51 2.3-.51 3.22 0l3.2 1.78c.96.53 1.7 1.8 1.7 2.9v3.39c0 1.09-.75 2.36-1.7 2.9l-3.2 1.78c-.46.25-1.03.38-1.61.38Zm-.88-11.81-3.2 1.78c-.49.27-.93 1.03-.93 1.58v3.39c0 .56.44 1.31.93 1.58l3.2 1.78c.46.25 1.3.25 1.76 0l3.2-1.78c.49-.27.93-1.03.93-1.58V10.3c0-.56-.44-1.31-.93-1.58l-3.2-1.78c-.46-.25-1.3-.25-1.76 0Z"
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
			d="M2 9V7c0-3 2-5 5-5h10c3 0 5 2 5 5v2M2 15v2c0 3 2 5 5 5h10c3 0 5-2 5-5v-2"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
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
			<path d="m6.703 9.258 5.3 3.07 5.26-3.05M12 17.77v-5.45"></path>
			<path
				d="m10.762 6.289-3.2 1.78c-.72.4-1.32 1.41-1.32 2.24v3.39c0 .83.59 1.84 1.32 2.24l3.2 1.78c.68.38 1.8.38 2.49 0l3.2-1.78c.72-.4 1.32-1.41 1.32-2.24v-3.39c0-.83-.59-1.84-1.32-2.24l-3.2-1.78c-.69-.39-1.81-.39-2.49 0Z"
			></path>
		</g>
	</svg>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
	name: 'I3DCubeScanIcon',
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
