# CSS Starter Kit

A simple CSS starter kit to get you started with your next project. It includes a basic CSS reset, css custom properties, typography, media queries, few components, dark mode, a grid system, and more.

## Features

- CSS Reset
- CSS Custom Properties
- Typography
- Media Queries
- Components
- Dark Mode
- Grid System

## Components

- Alert
- Badge
- Button
- Card
- Dropdown
- Form
- Modal
- Navbar
- Pagination
- Progress
- Table
- Tabs
- Toast

## Grid System

The grid system is based on the 12-column grid system. It uses CSS custom properties to define the grid layout.

```html
<div class="row">
  <div class="col-12">12</div>
</div>
<div class="row">
  <div class="col-6">6</div>
  <div class="col-6">6</div>
</div>
<div class="row">
  <div class="col-4">4</div>
  <div class="col-4">4</div>
  <div class="col-4">4</div>
</div>
<div class="row">
  <div class="col-3">3</div>
  <div class="col-3">3</div>
  <div class="col-3">3</div>
  <div class="col-3">3</div>
</div>
```

## Dark Mode

The dark mode is implemented using CSS custom properties and JavaScript. It uses the `prefers-color-scheme` media feature to detect the user's preferred color scheme.

```css
:root {
  --
    color-scheme: light dark;
}

@media (prefers-color-scheme: dark) {
  :root {
    --color-scheme: dark light;
  }
}

body {
  color-scheme: var(--color-scheme);
}
```

```vue
<template>
  <button @click="toggleDarkMode">Toggle Dark Mode</button>
</template>

<script setup>
const toggleDarkMode = () => {
  document.documentElement.classList.toggle('dark');
};
</script>
```

## Typography

The typography is based on the `Inter` font family. It includes the following font weights:

- 300
- 400
- 500
- 600
- 700

```css
body {
  font-family: 'Inter', sans-serif;
  font-weight: 400;
  font-size: 1rem;
  line-height: 1.5;
}
```

```html
    <h1>Heading 1</h1>
    <h2>Heading 2</h2>
    <h3>Heading 3</h3>
    <h4>Heading 4</h4>
    <h5>Heading 5</h5>
    <h6>Heading 6</h6>
    <p>Paragraph</p>
    <a href="#">Link</a>
    <button>Button</button>
    <label>Label</label>
    <input type="text" placeholder="Input" />
    <textarea placeholder="Textarea"></textarea>
```

## Media Queries

The media queries are based on the following breakpoints:

- 576px
- 768px
- 992px
- 1200px

```css
@media (min-width: 576px) {
  /* Styles */
}

@media (min-width: 768px) {
  /* Styles */
}

@media (min-width: 992px) {
  /* Styles */
}

@media (min-width: 1200px) {
  /* Styles */
}
```

```html
<div class="d-none d-sm-block">Hidden on mobile</div>
<div class="d-block d-sm-none">Hidden on desktop</div>
```

## CSS Custom Properties

The CSS custom properties are used to define the color scheme, grid layout, and spacing.

```css
:root {
  -- primary-color: #007bff;
    --secondary-color: #6c757d;
    --success-color: #28a745;
    --info-color: #17a2b8;
    --warning-color: #ffc107;
    --danger-color: #dc3545;
    --light-color: #f8f9fa;
    --dark-color: #343a40;
    --gray-color: #6c757d;
    --white-color: #fff;
    --black-color: #000;
    --grid-gap: 1rem;
    --container-max-width: 1140px;
}

body {
  color: var(--black-color);
  background-color: var(--white-color);
}
```

```html
<div class="container">Container</div>
<div class="row">
  <div class="col-6">Column</div>
  <div class="col-6">Column</div>
</div>
```

## CSS Reset

The CSS reset is based on the `normalize.css` library. It includes the following styles:

- Box-sizing
- Margin
- Padding
- List
- Table
- Form
- Button
- Image
- Typography

```css
html {
  box-sizing: border-box;
}

*,
*::before,
*::after {
  box-sizing: inherit;
}

ul[class],
ol[class] {
  padding: 0;
  margin: 0;
  list-style: none;
}

img {
  max-width: 100%;
  height: auto;
}

button,
input,
optgroup,
select,
textarea {
  padding: 0;
  margin: 0;
  font-family: inherit;
  font-size: inherit;
  line-height: inherit;
  color: inherit;
}
```

```html
<ul>
  <li>Item</li>
  <li>Item</li>
  <li>Item</li>
</ul>
```

## Setup

Make sure to install the dependencies:

```bash
# npm
npm install

# pnpm
pnpm install

# yarn
yarn install

# bun
bun install
```

## Development Server

Start the development server on `http://localhost:3000`:

```bash
# npm
npm run dev

# pnpm
pnpm run dev

# yarn
yarn dev

# bun
bun run dev
```

## Production

Build the application for production:

```bash
# npm
npm run build

# pnpm
pnpm run build

# yarn
yarn build

# bun
bun run build
```

Locally preview production build:

```bash
# npm
npm run preview

# pnpm
pnpm run preview

# yarn
yarn preview

# bun
bun run preview
```

Check out the [deployment documentation](https://nuxt.com/docs/getting-started/deployment) for more information.
