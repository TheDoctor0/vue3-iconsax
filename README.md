<article ><a name="user-content-readme-top"></a></p>

<div align="center">
  <h1 align="center"></a>iconsax for Vue3</h1>
  <p align="center">
    A total of 6000 icons in 6 different designs | <strong>Only supported for vue3</strong>
    <br>
    <br>
    <a href="https://vue-iconsax-preview.vercel.app/"><strong> Browse icons</strong></a>
  </p>
</div>

# About the Project

The features of this package include the following:

- 1000 icons in 6 different types
- Perfectly balance
- 24px grid-based
- Lightweight, powerful and easy to use
  <g-emoji class="g-emoji" alias="smile" fallback-src="https://github.githubassets.com/images/icons/emoji/unicode/1f604.png"><img class="emoji" alt="smile" src="https://github.githubassets.com/images/icons/emoji/unicode/1f604.png" width="20" height="20"></g-emoji>

<a href="https://vuejs.org/" rel="nofollow"><img src="https://www.cdnlogo.com/logos/v/92/vue-js.svg" width="70" height="70"></a>

# Installation

- Install Yarn package

```bash
yarn add vue3-iconsax
```

- Install NPM package

```bash
npm install vue3-iconsax
```

## Usage

Global registration:

```jsx
// main.js
import { VsxIcon } from "vue-iconsax";
const app = createApp(App);
// Dynamic icon component - Use PascalCase for iconName prop
app.component("VsxIcon", VsxIcon);
app.mount("#app");
```

```jsx
// App.vue
<template>
  // Dynamic icon component - Use PascalCase for iconName prop
  <VsxIcon :iconName="iconName" color="blue" size="50" type="linear" />
</template>

<script>
export default {
  props:['iconName']
};
</script>
```

Local registration:

```jsx
<template>
  <AaveIcon color="blue" size="50" type="linear" />
</template>

<script>
import { AaveIcon } from "vue3-iconsax";
export default {
  components: {
  AaveIcon
  },
};
</script>
```

## Props

| Prop       | Type                                                | Default        | Note                                                               |
| ---------- | --------------------------------------------------- | -------------- | ------------------------------------------------------------------ |
| `color`    | `string`                                            | `currentColor` | css color                                                          |
| `size`     | `number` `string`                                   | 24px           | size="24" or :size="24"                                            |
| `type`     | `Linear` `Outline` `TwoTone` `Bulk` `Broken` `Bold` | `Linear`       | icons styles                                                       |
| `iconName` | string                                              |                | iconName is only required with vsx-icon tag (Dynamic icon imports) |

</article >
