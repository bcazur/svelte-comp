# Intro

This is a template for creating an NPM package including:
- Svelte components
- TypeScript code

It is based on the standard [Svelte template](https://github.com/sveltejs/template) and the [Svelte typescript component template](https://github.com/mattjennings/svelte-typescript-component-template). The main benefit is being able to develop a component library independently, test it as a standalone app and then package it for reuse.
---

## Get started

Create a new component using this scaffolding.
```bash
npx degit bcazur/svelte-comp
```

Install the dependencies.
```bash
npm install
```

Run standalone web app using PlaceholderComponent.svelte.
```bash
npm run dev
```

Build library for reuse.
```bash
npm run build-lib
```
---
 
## Exporting additional components

Any new .svelte components must be exported from /src/index.ts.

```js
import PlaceholderComponent from './PlaceholderComponent.svelte';
import SecondComponent from './SecondComponent.svelte';

export {PlaceholderComponent, SecondComponent};
```
