# Introduction
This is a template for creating an NPM package including Svelte components and TypeScript code. 
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

## Using the component

To import the component in another Svelte app, you can either [publish to the NPM global repository](https://docs.npmjs.com/cli/v7/commands/npm-publish) or reference the package locally.

Note: the component will be imported in your /node_modules folder using the name specified in package.json, so make sure to change it before running npm install.

```bash
npm install ../my-svelte-component/ -D
```


## Exporting additional components

Any new .svelte components must be exported from /src/index.ts.

```js
import PlaceholderComponent from './PlaceholderComponent.svelte';
import SecondComponent from './SecondComponent.svelte';

export {PlaceholderComponent, SecondComponent};
```

---
## Aknowledgements
It is based on the standard [Svelte template](https://github.com/sveltejs/template) and the [Svelte typescript component template](https://github.com/mattjennings/svelte-typescript-component-template). The main benefit is being able to develop a component library independently, test it as a standalone app and then package it for reuse.
