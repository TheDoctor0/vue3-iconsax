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
			d="M19.14 7.72C19.43 8.47 20.15 9 21 9c1.1 0 2-.9 2-2s-.9-2-2-2c-.85 0-1.57.53-1.86 1.28-.05-.01-.09-.03-.14-.03h-4V5.5c0-.82-.68-1.5-1.5-1.5h-3C9.68 4 9 4.68 9 5.5v.75H5c-.05 0-.09.02-.14.03A1.992 1.992 0 0 0 3 5c-1.1 0-2 .9-2 2s.9 2 2 2c.85 0 1.57-.53 1.86-1.28.05.01.09.03.14.03h2.57c-2.05 1.52-3.32 4.04-3.32 6.75 0 .17.01.33.03.5H4c-.83 0-1.5.67-1.5 1.5v2c0 .83.67 1.5 1.5 1.5h2c.22 0 .42-.05.61-.14.52-.22.89-.75.89-1.36v-2c0-.83-.67-1.5-1.5-1.5h-.23c0-.03.01-.06.01-.09-.02-.14-.02-.27-.02-.41 0-2.47 1.27-4.73 3.26-5.9.04.77.69 1.4 1.48 1.4h3c.79 0 1.44-.63 1.49-1.4 1.99 1.17 3.26 3.44 3.26 5.9 0 .14-.01.27-.02.41 0 .03.01.06.01.09H18c-.83 0-1.5.67-1.5 1.5v2c0 .61.37 1.14.89 1.36.19.09.39.14.61.14h2c.83 0 1.5-.67 1.5-1.5v-2c0-.83-.67-1.5-1.5-1.5h-.28c.02-.17.03-.33.03-.5 0-2.71-1.27-5.23-3.32-6.75H19c.05 0 .09-.02.14-.03Z"
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
			d="M3 9a2 2 0 1 0 0-4 2 2 0 0 0 0 4ZM21 9a2 2 0 1 0 0-4 2 2 0 0 0 0 4ZM19 7h-4M9 7H5M7.5 16.5v2c0 .61-.37 1.14-.89 1.36A1.4 1.4 0 0 1 6 20H4c-.83 0-1.5-.67-1.5-1.5v-2c0-.83.67-1.5 1.5-1.5h2c.83 0 1.5.67 1.5 1.5ZM21.5 16.5v2c0 .83-.67 1.5-1.5 1.5h-2a1.4 1.4 0 0 1-.61-.14c-.52-.22-.89-.75-.89-1.36v-2c0-.83.67-1.5 1.5-1.5h2c.83 0 1.5.67 1.5 1.5ZM15 5.5v3c0 .82-.68 1.5-1.5 1.5h-3C9.68 10 9 9.32 9 8.5v-3c0-.82.68-1.5 1.5-1.5h3c.82 0 1.5.68 1.5 1.5ZM15 7.73c1.31.66 2.39 1.74 3.1 3.08"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M5.03 15c-.02-.17-.03-.33-.03-.5 0-2.99 1.63-5.57 4-6.77"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
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
			d="M3 9a2 2 0 1 0 0-4 2 2 0 0 0 0 4ZM21 9a2 2 0 1 0 0-4 2 2 0 0 0 0 4ZM7.5 16.5v2c0 .61-.37 1.14-.89 1.36A1.4 1.4 0 0 1 6 20H4c-.83 0-1.5-.67-1.5-1.5v-2c0-.83.67-1.5 1.5-1.5h2c.83 0 1.5.67 1.5 1.5ZM21.5 16.5v2c0 .83-.67 1.5-1.5 1.5h-2a1.4 1.4 0 0 1-.61-.14c-.52-.22-.89-.75-.89-1.36v-2c0-.83.67-1.5 1.5-1.5h2c.83 0 1.5.67 1.5 1.5ZM15 5.5v3c0 .82-.68 1.5-1.5 1.5h-3C9.68 10 9 9.32 9 8.5v-3c0-.82.68-1.5 1.5-1.5h3c.82 0 1.5.68 1.5 1.5Z"
			:fill="color"
		></path>
		<g
			opacity=".4"
			:fill="color"
		>
			<path
				opacity=".4"
				d="M9 6.25H5c-.41 0-.75.34-.75.75s.34.75.75.75h2.57c-2.05 1.52-3.32 4.04-3.32 6.75 0 .2.01.39.04.59.04.38.37.66.74.66h.09c.41-.05.71-.42.66-.83-.02-.14-.02-.27-.02-.41 0-2.6 1.41-5 3.59-6.1a.75.75 0 0 0 .33-1.01c-.01-.01-.02-.02-.02-.03.06-.11.11-.23.11-.36-.02-.42-.36-.76-.77-.76ZM16.43 7.75H19c.41 0 .75-.34.75-.75s-.34-.75-.75-.75h-4c-.41 0-.75.34-.75.75 0 .13.04.25.11.36-.01.01-.02.02-.02.03a.75.75 0 0 0 .33 1.01c2.18 1.1 3.59 3.5 3.59 6.1 0 .14-.01.27-.02.41-.05.41.25.78.66.83h.09c.38 0 .7-.28.74-.66.02-.2.04-.39.04-.59-.02-2.7-1.29-5.22-3.34-6.74Z"
			></path>
		</g>
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
			stroke-miterlimit="10"
			:stroke-width="strokeWidth"
			d="M3 9a2 2 0 100-4 2 2 0 000 4zM21 9a2 2 0 100-4 2 2 0 000 4zM19 7h-4M9 7H5M7.5 16.5v2c0 .61-.37 1.14-.89 1.36A1.4 1.4 0 016 20H4c-.83 0-1.5-.67-1.5-1.5v-2c0-.83.67-1.5 1.5-1.5h2c.83 0 1.5.67 1.5 1.5zM21.5 16.5v2c0 .83-.67 1.5-1.5 1.5h-2a1.4 1.4 0 01-.61-.14c-.52-.22-.89-.75-.89-1.36v-2c0-.83.67-1.5 1.5-1.5h2c.83 0 1.5.67 1.5 1.5zM15 5.5v3c0 .82-.68 1.5-1.5 1.5h-3C9.68 10 9 9.32 9 8.5v-3c0-.82.68-1.5 1.5-1.5h3c.82 0 1.5.68 1.5 1.5z"
		></path>
		<path
			:stroke="color"
			stroke-linecap="round"
			stroke-linejoin="round"
			stroke-miterlimit="10"
			:stroke-width="strokeWidth"
			d="M15 7.73c2.37 1.2 4 3.78 4 6.77 0 .17-.01.33-.03.5M5.03 15c-.02-.17-.03-.33-.03-.5 0-2.99 1.63-5.57 4-6.77"
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
			d="M3 9.75C1.48 9.75.25 8.52.25 7S1.48 4.25 3 4.25 5.75 5.48 5.75 7 4.52 9.75 3 9.75Zm0-4a1.25 1.25 0 1 0 0 2.5 1.25 1.25 0 0 0 0-2.5ZM21 9.75c-1.52 0-2.75-1.23-2.75-2.75S19.48 4.25 21 4.25 23.75 5.48 23.75 7 22.52 9.75 21 9.75Zm0-4a1.25 1.25 0 1 0 0 2.5 1.25 1.25 0 0 0 0-2.5Z"
			:fill="color"
		></path>
		<path
			d="M19 7.75h-4c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h4c.41 0 .75.34.75.75s-.34.75-.75.75ZM9 7.75H5c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h4c.41 0 .75.34.75.75s-.34.75-.75.75ZM6 20.75H4c-1.24 0-2.25-1.01-2.25-2.25v-2c0-1.24 1.01-2.25 2.25-2.25h2c1.24 0 2.25 1.01 2.25 2.25v2c0 .9-.53 1.7-1.35 2.05-.27.13-.58.2-.9.2Zm-2-5c-.41 0-.75.34-.75.75v2c0 .41.34.75.75.75h2c.1 0 .19-.02.29-.07.29-.12.46-.39.46-.68v-2c0-.41-.34-.75-.75-.75H4ZM20 20.75h-2c-.32 0-.63-.07-.93-.21-.79-.33-1.32-1.14-1.32-2.04v-2c0-1.24 1.01-2.25 2.25-2.25h2c1.24 0 2.25 1.01 2.25 2.25v2c0 1.24-1.01 2.25-2.25 2.25Zm-2-5c-.41 0-.75.34-.75.75v2c0 .29.17.56.43.67.13.06.22.08.32.08h2c.41 0 .75-.34.75-.75v-2c0-.41-.34-.75-.75-.75h-2Z"
			:fill="color"
		></path>
		<path
			d="M13.5 10.75h-3c-1.24 0-2.25-1.01-2.25-2.25v-3c0-1.24 1.01-2.25 2.25-2.25h3c1.24 0 2.25 1.01 2.25 2.25v3c0 1.24-1.01 2.25-2.25 2.25Zm-3-6c-.41 0-.75.34-.75.75v3c0 .41.34.75.75.75h3c.41 0 .75-.34.75-.75v-3c0-.41-.34-.75-.75-.75h-3Z"
			:fill="color"
		></path>
		<path
			d="M18.97 15.75h-.09a.751.751 0 0 1-.66-.83c.02-.14.02-.27.02-.41 0-2.6-1.41-5-3.59-6.1a.75.75 0 1 1 .68-1.34c2.68 1.36 4.41 4.28 4.41 7.44 0 .2-.01.39-.04.59-.03.37-.35.65-.73.65ZM5.03 15.749c-.38 0-.7-.28-.74-.66-.02-.2-.04-.39-.04-.59 0-3.16 1.73-6.08 4.41-7.44a.75.75 0 0 1 1.01.33c.19.37.04.82-.33 1.01-2.18 1.1-3.59 3.5-3.59 6.1 0 .14.01.27.02.41.05.41-.25.78-.66.83-.02.01-.05.01-.08.01Z"
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
			d="M3 9a2 2 0 1 0 0-4 2 2 0 0 0 0 4ZM21 9a2 2 0 1 0 0-4 2 2 0 0 0 0 4ZM19 7h-4M9 7H5M7.5 16.5v2c0 .61-.37 1.14-.89 1.36A1.4 1.4 0 0 1 6 20H4c-.83 0-1.5-.67-1.5-1.5v-2c0-.83.67-1.5 1.5-1.5h2c.83 0 1.5.67 1.5 1.5ZM21.5 16.5v2c0 .83-.67 1.5-1.5 1.5h-2a1.4 1.4 0 0 1-.61-.14c-.52-.22-.89-.75-.89-1.36v-2c0-.83.67-1.5 1.5-1.5h2c.83 0 1.5.67 1.5 1.5ZM15 5.5v3c0 .82-.68 1.5-1.5 1.5h-3C9.68 10 9 9.32 9 8.5v-3c0-.82.68-1.5 1.5-1.5h3c.82 0 1.5.68 1.5 1.5Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M15 7.73c2.37 1.2 4 3.78 4 6.77 0 .17-.01.33-.03.5M5.03 15c-.02-.17-.03-.33-.03-.5 0-2.99 1.63-5.57 4-6.77"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
	</svg>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
	name: 'BezierIcon',
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
