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
			d="M21.091 6.98c-.85-.94-2.27-1.41-4.33-1.41h-.24v-.04c0-1.68 0-3.76-3.76-3.76h-1.52c-3.76 0-3.76 2.09-3.76 3.76v.05h-.24c-2.07 0-3.48.47-4.33 1.41-.99 1.1-.96 2.58-.86 3.59l.01.07.077.813c.015.15.095.285.221.367.24.157.641.416.882.55.14.09.29.17.44.25 1.71.94 3.59 1.57 5.5 1.88.09.94.5 2.04 2.69 2.04s2.62-1.09 2.69-2.06c2.04-.33 4.01-1.04 5.79-2.08.06-.03.1-.06.15-.09.397-.225.808-.501 1.183-.772a.493.493 0 0 0 .201-.346l.016-.143.05-.47c.01-.06.01-.11.02-.18.08-1.01.06-2.39-.88-3.43Zm-8 6.85c0 1.06 0 1.22-1.23 1.22s-1.23-.19-1.23-1.21v-1.26h2.46v1.25Zm-4.18-8.26v-.04c0-1.7 0-2.33 2.33-2.33h1.52c2.33 0 2.33.64 2.33 2.33v.05h-6.18v-.01Z"
			:fill="color"
		></path>
		<path
			d="M20.873 13.735a.509.509 0 0 1 .726.502l-.36 3.954c-.21 2-1.03 4.04-5.43 4.04H8.19c-4.4 0-5.22-2.04-5.43-4.03l-.34-3.748a.508.508 0 0 1 .716-.506c1.14.516 3.242 1.43 4.541 1.77a.57.57 0 0 1 .37.315c.607 1.298 1.923 1.989 3.824 1.989 1.882 0 3.215-.718 3.824-2.019a.571.571 0 0 1 .37-.315c1.379-.363 3.618-1.385 4.81-1.952Z"
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
			d="m21.37 14 .34-3.57C21.97 7.99 21.27 6 17 6H7c-4.27 0-4.97 1.99-4.7 4.43l.75 8C3.26 20.39 3.98 22 8 22h8c4.02 0 4.74-1.61 4.95-3.57M8 6v-.8C8 3.43 8 2 11.2 2h1.6C16 2 16 3.43 16 5.2V6"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M14 13v1.02c0 1.09-.01 1.98-2 1.98-1.98 0-2-.88-2-1.97V13c0-1 0-1 1-1h2c1 0 1 0 1 1ZM21.65 11A16.484 16.484 0 0 1 14 14.02"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M2.621 11.27c2.25 1.54 4.79 2.47 7.38 2.76"
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
			d="M21.091 6.98c-.85-.94-2.27-1.41-4.33-1.41h-.24v-.04c0-1.68 0-3.76-3.76-3.76h-1.52c-3.76 0-3.76 2.09-3.76 3.76v.05h-.24c-2.07 0-3.48.47-4.33 1.41-.99 1.1-.96 2.58-.86 3.59l.01.07.1 1.05c.01.01.03.03.05.04.33.22.67.44 1.03.64.14.09.29.17.44.25 1.71.94 3.59 1.57 5.5 1.88.09.94.5 2.04 2.69 2.04s2.62-1.09 2.69-2.06c2.04-.33 4.01-1.04 5.79-2.08.06-.03.1-.06.15-.09.46-.26.89-.54 1.31-.85a.12.12 0 0 0 .05-.05l.04-.36.05-.47c.01-.06.01-.11.02-.18.08-1.01.06-2.39-.88-3.43Zm-8 6.85c0 1.06 0 1.22-1.23 1.22s-1.23-.19-1.23-1.21v-1.26h2.46v1.25Zm-4.18-8.26v-.04c0-1.7 0-2.33 2.33-2.33h1.52c2.33 0 2.33.64 2.33 2.33v.05h-6.18v-.01Z"
			:fill="color"
		></path>
		<path
			opacity=".4"
			d="m20.5 12.298-.15.09a17.037 17.037 0 0 1-5.79 2.08c-.08.96-.5 2.06-2.69 2.06s-2.61-1.09-2.69-2.04c-1.91-.3-3.79-.93-5.5-1.88-.15-.08-.3-.16-.44-.25-.36-.2-.7-.42-1.03-.64-.02-.01-.04-.03-.05-.04l.61 6.51c.21 1.99 1.03 4.04 5.43 4.04h7.62c4.4 0 5.22-2.05 5.43-4.05l.63-6.78a.12.12 0 0 1-.05.05c-.43.31-.87.6-1.33.85Z"
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
			d="M8 22h8c4.02 0 4.74-1.61 4.95-3.57l.75-8C21.97 7.99 21.27 6 17 6H7c-4.27 0-4.97 1.99-4.7 4.43l.75 8C3.26 20.39 3.98 22 8 22ZM8 6v-.8C8 3.43 8 2 11.2 2h1.6C16 2 16 3.43 16 5.2V6"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M14 13v1.02c0 1.09-.01 1.98-2 1.98-1.98 0-2-.88-2-1.97V13c0-1 0-1 1-1h2c1 0 1 0 1 1ZM21.65 11A16.484 16.484 0 0 1 14 14.02M2.62 11.27c2.25 1.54 4.79 2.47 7.38 2.76"
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
		v-else-if="type === 'outline'"
	>
		<path
			d="M15.998 22.752h-8c-4.62 0-5.48-2.15-5.7-4.24l-.75-8.01c-.11-1.05-.14-2.6.9-3.76.9-1 2.39-1.48 4.55-1.48h10c2.17 0 3.66.49 4.55 1.48 1.04 1.16 1.01 2.71.9 3.77l-.75 7.99c-.22 2.1-1.08 4.25-5.7 4.25Zm-9-16c-1.69 0-2.85.33-3.44.99-.49.54-.65 1.37-.52 2.61l.75 8.01c.17 1.58.6 2.89 4.21 2.89h8c3.6 0 4.04-1.31 4.21-2.9l.75-7.99c.13-1.25-.03-2.08-.52-2.62-.59-.66-1.75-.99-3.44-.99h-10Z"
			:fill="color"
		></path>
		<path
			d="M16 6.75c-.41 0-.75-.34-.75-.75v-.8c0-1.78 0-2.45-2.45-2.45h-1.6c-2.45 0-2.45.67-2.45 2.45V6c0 .41-.34.75-.75.75s-.75-.34-.75-.75v-.8c0-1.76 0-3.95 3.95-3.95h1.6c3.95 0 3.95 2.19 3.95 3.95V6c0 .41-.34.75-.75.75ZM12 16.75c-2.75 0-2.75-1.7-2.75-2.72V13c0-1.41.34-1.75 1.75-1.75h2c1.41 0 1.75.34 1.75 1.75v1c0 1.04 0 2.75-2.75 2.75Zm-1.25-4v1.28c0 1.03 0 1.22 1.25 1.22s1.25-.16 1.25-1.23v-1.27h-2.5Z"
			:fill="color"
		></path>
		<path
			d="M14 14.768c-.37 0-.7-.28-.74-.66-.05-.41.24-.79.65-.84 2.64-.33 5.17-1.33 7.3-2.88.33-.25.8-.17 1.05.17.24.33.17.8-.17 1.05-2.34 1.7-5.1 2.79-8 3.16H14ZM10 14.78h-.09c-2.74-.31-5.41-1.31-7.72-2.89a.753.753 0 0 1-.2-1.04c.23-.34.7-.43 1.04-.2 2.11 1.44 4.54 2.35 7.04 2.64.41.05.71.42.66.83-.03.38-.35.66-.73.66Z"
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
			d="M8 22h8c4.02 0 4.74-1.61 4.95-3.57l.75-8C21.97 7.99 21.27 6 17 6H7c-4.27 0-4.97 1.99-4.7 4.43l.75 8C3.26 20.39 3.98 22 8 22Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M8 6v-.8C8 3.43 8 2 11.2 2h1.6C16 2 16 3.43 16 5.2V6"
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
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		>
			<path
				d="M14 13v1.02c0 1.09-.01 1.98-2 1.98-1.98 0-2-.88-2-1.97V13c0-1 0-1 1-1h2c1 0 1 0 1 1ZM21.65 11A16.484 16.484 0 0 1 14 14.02M2.617 11.27c2.25 1.54 4.79 2.47 7.38 2.76"
			></path>
		</g>
	</svg>
</template>
<script lang="ts">
import { defineComponent } from "vue";
export default defineComponent({
	name: 'BriefcaseIcon',
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
