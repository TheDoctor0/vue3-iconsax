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
			d="M5 15c-1.02 0-1.96.39-2.67 1.03-.16.14-.31.29-.44.46A3.96 3.96 0 0 0 1 19c0 2.21 1.8 4 4 4 .96 0 1.83-.34 2.52-.89.56-.47 1-1.08 1.24-1.78.16-.41.24-.86.24-1.33 0-2.2-1.79-4-4-4Zm2.4 3.23c0 .28-.22.49-.49.49s-.49-.21-.49-.49v-.1c0-.11-.08-.2-.19-.2h-2a.483.483 0 0 1-.43.72c-.12 0-.25-.05-.34-.14l-.72-.72a.645.645 0 0 1-.11-.16.585.585 0 0 1 0-.37c.03-.05.06-.12.11-.16l.72-.71c.19-.2.5-.2.68 0 .16.15.18.39.08.57h2.01c.64 0 1.16.52 1.16 1.17v.1h.01Zm-1.2 3.53a.46.46 0 0 1-.35-.14.471.471 0 0 1-.08-.57H3.76c-.64 0-1.16-.52-1.16-1.17v-.1c0-.28.22-.49.49-.49s.49.21.49.49v.1c0 .11.08.2.19.2h2.01c-.1-.19-.08-.42.08-.58.19-.19.5-.19.68 0l.72.72c.04.04.08.1.11.16.04.12.04.25 0 .37-.03.05-.07.11-.11.15l-.72.71c-.09.1-.22.15-.34.15ZM14.85 3.95v3.8h-1.5v-3.8c0-.27-.24-.4-.4-.4-.05 0-.1.01-.15.03L4.87 6.57c-.53.2-.87.7-.87 1.27v.67c-.91.68-1.5 1.77-1.5 3V7.84c0-1.19.73-2.25 1.84-2.67l7.94-3c.22-.08.45-.12.67-.12 1 0 1.9.81 1.9 1.9ZM21.5 14.5v1a.5.5 0 0 1-.49.5h-1.46c-.53 0-1.01-.39-1.05-.91-.03-.31.09-.6.29-.8a.95.95 0 0 1 .7-.29H21c.29.01.5.23.5.5Z"
			:fill="color"
		></path>
		<path
			d="M19.48 12.95h1.02c.55 0 1-.45 1-1v-.44c0-2.07-1.69-3.76-3.76-3.76H6.26c-.85 0-1.63.28-2.26.76-.91.68-1.5 1.77-1.5 3v1.78c0 .38.4.62.76.5.56-.19 1.15-.29 1.74-.29 3.03 0 5.5 2.47 5.5 5.5 0 .72-.19 1.51-.49 2.21-.16.36.09.79.48.79h7.25c2.07 0 3.76-1.69 3.76-3.76v-.19c0-.55-.45-1-1-1h-.87c-.96 0-1.88-.59-2.13-1.52-.2-.76.04-1.5.54-1.98.37-.38.88-.6 1.44-.6Zm-5.48-.2H9c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h5c.41 0 .75.34.75.75s-.34.75-.75.75Z"
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
			d="M2.5 13.24v-1.73c0-2.07 1.69-3.76 3.76-3.76h11.48c2.07 0 3.76 1.69 3.76 3.76v1.44h-2.02c-.56 0-1.07.22-1.44.6-.42.41-.66 1-.6 1.63.09 1.08 1.08 1.87 2.16 1.87h1.9v1.19c0 2.07-1.69 3.76-3.76 3.76h-5.48"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22.559 13.97v2.06c0 .55-.44 1-1 1.02h-1.96c-1.08 0-2.07-.79-2.16-1.87-.06-.63.18-1.22.6-1.63.37-.38.88-.6 1.44-.6h2.08c.56.02 1 .47 1 1.02ZM7 12h7"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M3 16.5h5.34c.64 0 1.16.52 1.16 1.16v1.28"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M4.22 15.281 3 16.501l1.22 1.22M9.5 21.78H4.16c-.64 0-1.16-.52-1.16-1.16v-1.28"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m8.281 23.003 1.22-1.22-1.22-1.22"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M12.281 2.171a1.9 1.9 0 0 1 2.57 1.78v3.8M2.5 12.412v-4.57c0-1.19.73-2.25 1.84-2.67l3.97-1.5"
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
			d="M19.48 12.95h2.02v-1.44c0-2.07-1.69-3.76-3.76-3.76H6.26c-2.07 0-3.76 1.69-3.76 3.76v3.65c.79-.72 1.85-1.16 3-1.16a4.5 4.5 0 0 1 4.5 4.5c0 .53-.09 1.03-.26 1.5-.27.79-.77 1.47-1.4 2h9.4c2.07 0 3.76-1.69 3.76-3.76v-1.19h-1.9c-1.08 0-2.07-.79-2.16-1.87-.06-.63.18-1.22.6-1.63.37-.38.88-.6 1.44-.6Z"
			:fill="color"
		></path>
		<path
			d="M5.5 14c-1.15 0-2.21.44-3 1.16A4.428 4.428 0 0 0 1 18.5 4.5 4.5 0 0 0 5.5 23c1.08 0 2.06-.38 2.84-1 .63-.53 1.13-1.21 1.4-2 .17-.47.26-.97.26-1.5A4.5 4.5 0 0 0 5.5 14Zm2.7 3.63c0 .31-.25.55-.55.55-.3 0-.55-.24-.55-.55v-.11c0-.12-.09-.22-.21-.22H4.63a.547.547 0 0 1-.48.81c-.14 0-.28-.06-.38-.16l-.81-.81a.567.567 0 0 1-.12-.18.607.607 0 0 1 0-.42c.03-.06.07-.13.12-.18l.81-.8c.21-.22.56-.22.77 0 .18.17.2.44.09.64h2.26c.72 0 1.31.59 1.31 1.32v.11ZM6.85 21.6c-.15 0-.29-.05-.39-.16a.532.532 0 0 1-.09-.64H4.11c-.72 0-1.31-.59-1.31-1.32v-.11c0-.31.25-.55.55-.55.3 0 .55.24.55.55v.11c0 .12.09.22.21.22h2.26a.547.547 0 0 1 .09-.65.55.55 0 0 1 .77 0l.81.81c.05.05.09.11.12.18.05.13.05.28 0 .42-.03.06-.07.13-.12.18l-.81.8c-.1.11-.24.16-.38.16ZM14.85 3.952v3.8H6.26c-2.07 0-3.76 1.69-3.76 3.76v-3.67c0-1.19.73-2.25 1.84-2.67l7.94-3c1.24-.46 2.57.45 2.57 1.78ZM22.559 13.97v2.06c0 .55-.44 1-1 1.02h-1.96c-1.08 0-2.07-.79-2.16-1.87-.06-.63.18-1.22.6-1.63.37-.38.88-.6 1.44-.6h2.08c.56.02 1 .47 1 1.02ZM14 12.75H7c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h7c.41 0 .75.34.75.75s-.34.75-.75.75Z"
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
			d="M2.5 13.24v-1.73c0-2.07 1.69-3.76 3.76-3.76h11.48c2.07 0 3.76 1.69 3.76 3.76v1.44h-2.02c-.56 0-1.07.22-1.44.6-.42.41-.66 1-.6 1.63.09 1.08 1.08 1.87 2.16 1.87h1.9v1.19c0 2.07-1.69 3.76-3.76 3.76h-5.48"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M2.5 12.41V7.84c0-1.19.73-2.25 1.84-2.67l7.94-3a1.9 1.9 0 0 1 2.57 1.78v3.8M22.559 13.97v2.06c0 .55-.44 1-1 1.02h-1.96c-1.08 0-2.07-.79-2.16-1.87-.06-.63.18-1.22.6-1.63.37-.38.88-.6 1.44-.6h2.08c.56.02 1 .47 1 1.02ZM7 12h7"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M3 16.5h5.34c.64 0 1.16.52 1.16 1.16v1.28"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M4.22 15.28 3 16.5l1.22 1.22M9.5 21.78H4.16c-.64 0-1.16-.52-1.16-1.16v-1.28"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m8.281 23 1.22-1.22-1.22-1.22"
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
			d="M17.742 22.75h-5.48c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h5.48c1.66 0 3.01-1.35 3.01-3.01v-.44h-1.15c-1.51 0-2.79-1.12-2.91-2.56-.08-.83.22-1.64.82-2.23.51-.52 1.21-.81 1.96-.81h1.27v-.69c0-1.66-1.35-3.01-3.01-3.01H6.252c-1.66 0-3.01 1.35-3.01 3.01v1.73c0 .41-.34.75-.75.75s-.75-.34-.75-.75v-1.73c0-2.49 2.02-4.51 4.51-4.51h11.48c2.49 0 4.51 2.02 4.51 4.51v1.44c0 .41-.34.75-.75.75h-2.02c-.35 0-.67.13-.9.37-.29.28-.43.66-.39 1.04.06.66.69 1.19 1.41 1.19h1.9c.41 0 .75.34.75.75v1.19a4.496 4.496 0 0 1-4.5 4.51Z"
			:fill="color"
		></path>
		<path
			d="M2.5 13.16c-.41 0-.75-.34-.75-.75V7.84c0-1.49.94-2.84 2.33-3.37l7.94-3c.82-.31 1.73-.2 2.44.3.72.5 1.14 1.31 1.14 2.18v3.8c0 .41-.34.75-.75.75s-.75-.34-.75-.75v-3.8c0-.38-.18-.73-.5-.95-.32-.22-.7-.27-1.06-.13l-7.94 3c-.81.31-1.36 1.1-1.36 1.97v4.57c.01.42-.33.75-.74.75ZM19.599 17.8c-1.51 0-2.79-1.12-2.91-2.56-.08-.83.22-1.64.82-2.23.51-.52 1.21-.81 1.96-.81h2.08c.99.03 1.75.81 1.75 1.77v2.06c0 .96-.76 1.74-1.72 1.77h-1.98Zm1.93-4.1h-2.05c-.35 0-.67.13-.9.37-.29.28-.43.66-.39 1.04.06.66.69 1.19 1.41 1.19h1.96c.13 0 .25-.12.25-.27v-2.06c0-.15-.12-.26-.28-.27Z"
			:fill="color"
		></path>
		<path
			d="M14 12.75H7c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h7c.41 0 .75.34.75.75s-.34.75-.75.75ZM9.5 19.69c-.41 0-.75-.34-.75-.75v-1.28c0-.22-.18-.41-.41-.41H3c-.41 0-.75-.34-.75-.75s.34-.75.75-.75h5.34c1.05 0 1.91.86 1.91 1.91v1.28c0 .41-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M4.221 18.469c-.19 0-.38-.07-.53-.22l-1.22-1.22a.755.755 0 0 1 0-1.06l1.22-1.22c.29-.29.77-.29 1.06 0 .29.29.29.77 0 1.06l-.69.69.69.69c.29.29.29.77 0 1.06-.15.15-.34.22-.53.22ZM9.5 22.53H4.16c-1.05 0-1.91-.86-1.91-1.91v-1.28c0-.41.34-.75.75-.75s.75.34.75.75v1.28c0 .22.18.41.41.41H9.5c.41 0 .75.34.75.75s-.34.75-.75.75Z"
			:fill="color"
		></path>
		<path
			d="M8.279 23.75c-.19 0-.38-.07-.53-.22a.755.755 0 0 1 0-1.06l.69-.69-.69-.69a.754.754 0 0 1 0-1.06c.29-.29.77-.29 1.06 0l1.22 1.22c.29.29.29.77 0 1.06l-1.22 1.22c-.14.15-.34.22-.53.22Z"
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
			d="M2.5 13.24v-1.73c0-2.07 1.69-3.76 3.76-3.76h11.48c2.07 0 3.76 1.69 3.76 3.76v1.44h-2.02c-.56 0-1.07.22-1.44.6-.42.41-.66 1-.6 1.63.09 1.08 1.08 1.87 2.16 1.87h1.9v1.19c0 2.07-1.69 3.76-3.76 3.76h-5.48"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M2.5 12.411v-4.57c0-1.19.73-2.25 1.84-2.67l7.94-3a1.9 1.9 0 0 1 2.57 1.78v3.8"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M22.559 13.97v2.06c0 .55-.44 1-1 1.02h-1.96c-1.08 0-2.07-.79-2.16-1.87-.06-.63.18-1.22.6-1.63.37-.38.88-.6 1.44-.6h2.08c.56.02 1 .47 1 1.02Z"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			opacity=".4"
			d="M7 12h7"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M3 16.5h5.34c.64 0 1.16.52 1.16 1.16v1.28"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="M4.22 15.281 3 16.501l1.22 1.22M9.5 21.78H4.16c-.64 0-1.16-.52-1.16-1.16v-1.28"
			:stroke="color"
			:stroke-width="strokeWidth"
			stroke-miterlimit="10"
			stroke-linecap="round"
			stroke-linejoin="round"
		></path>
		<path
			d="m8.281 23.003 1.22-1.22-1.22-1.22"
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
	name: 'EmptyWalletChangeIcon',
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
