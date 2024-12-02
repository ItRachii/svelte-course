# Svelte + Vite

This template should help get you started developing with Svelte in Vite.

## Recommended IDE Setup

[VS Code](https://code.visualstudio.com/) + [Svelte](https://marketplace.visualstudio.com/items?itemName=svelte.svelte-vscode).

## Need an official Svelte framework?

Check out [SvelteKit](https://github.com/sveltejs/kit#readme), which is also powered by Vite. Deploy anywhere with its serverless-first approach and adapt to various platforms, with out of the box support for TypeScript, SCSS, and Less, and easily-added support for mdsvex, GraphQL, PostCSS, Tailwind CSS, and more.

## Technical considerations

**Why use this over SvelteKit?**

- It brings its own routing solution which might not be preferable for some users.
- It is first and foremost a framework that just happens to use Vite under the hood, not a Vite app.
  `vite dev` and `vite build` wouldn't work in a SvelteKit environment, for example.

This template contains as little as possible to get started with Vite + Svelte, while taking into account the developer experience with regards to HMR and intellisense. It demonstrates capabilities on par with the other `create-vite` templates and is a good starting point for beginners dipping their toes into a Vite + Svelte project.

Should you later need the extended capabilities and extensibility provided by SvelteKit, the template has been structured similarly to SvelteKit so that it is easy to migrate.

**Why `global.d.ts` instead of `compilerOptions.types` inside `jsconfig.json` or `tsconfig.json`?**

Setting `compilerOptions.types` shuts out all other types not explicitly listed in the configuration. Using triple-slash references keeps the default TypeScript setting of accepting type information from the entire workspace, while also adding `svelte` and `vite/client` type information.

**Why include `.vscode/extensions.json`?**

Other templates indirectly recommend extensions via the README, but this file allows VS Code to prompt the user to install the recommended extension upon opening the project.

**Why enable `checkJs` in the JS template?**

It is likely that most cases of changing variable types in runtime are likely to be accidental, rather than deliberate. This provides advanced typechecking out of the box. Should you like to take advantage of the dynamically-typed nature of JavaScript, it is trivial to change the configuration.

**Why is HMR not preserving my local component state?**

HMR state preservation comes with a number of gotchas! It has been disabled by default in both `svelte-hmr` and `@sveltejs/vite-plugin-svelte` due to its often surprising behavior. You can read the details [here](https://github.com/rixo/svelte-hmr#svelte-hmr).

If you have state that's important to retain within a component, consider creating an external store which would not be replaced by HMR.

```js
// store.js
// An extremely simple external store
import { writable } from 'svelte/store'
export default writable(0)
```


## Course Content

**Section 1: Introduction**

1. [Write less code](https://svelte.dev/blog/write-less-code)
2. [Frameworks without the frameworks](https://svelte.dev/blog/frameworks-without-the-framework)
3. [Virtual DOM](https://svelte.dev/blog/virtual-dom-is-pure-overhead)
4. [sveltesociety.dev](https://www.sveltesociety.dev/packages)
5. [REPL](https://svelte.dev/playground/hello-world?version=5.2.10)

**Section 2: Getting Started With Svelte**

1. [Getting Started Docs](https://svelte.dev/docs/svelte/overview)
2. [Creating a Svelte Vite Template](https://github.com/alialaa/svelte-course/tree/svelte-vite-template)
3. [Svelte Components Basic Structure](https://github.com/alialaa/svelte-course/tree/first-component)
4. [Counter Component](https://github.com/alialaa/svelte-course/tree/simple-counter)
5. [State](https://github.com/alialaa/svelte-course/tree/reactive-statements)
6. [Reactive Statements - 1](https://github.com/alialaa/svelte-course/tree/reactive-gotcha-1)
7. [Reactive Statements - 2](https://github.com/alialaa/svelte-course/tree/reactive-gotcha-2)
8. [Component Prop](https://github.com/alialaa/svelte-course/tree/props)

**Section 3: Exploring More Svelte By Creating a Button Component**

1. [Accessing Component Child with Slot](https://github.com/alialaa/svelte-course/tree/button-component-1)
2. [svelte-preprocessor](https://github.com/sveltejs/svelte-preprocess)
3. [Adding Svelte Preprocessor](https://github.com/alialaa/svelte-course/tree/adding-scss)
4. [Class Directive](https://github.com/alialaa/svelte-course/tree/class-directive)
5. [Style Directive in-line](https://github.com/alialaa/svelte-course/tree/style-directive)
6. [Style Directive in-line variable](https://github.com/alialaa/svelte-course/tree/style-directive-css-vars)
7. [Named Slots](https://github.com/alialaa/svelte-course/tree/named-slots)
8. [Svelte Icon](https://github.com/Introvertuous/svelte-icons)
9. [Slot Props](https://github.com/alialaa/svelte-course/tree/slot-props)
10. [Event Forwarding and Modifier](https://github.com/alialaa/svelte-course/tree/button-events)
11. [Event Modifier Documentation](https://svelte.dev/docs#template-syntax-element-directives-on-eventname)
12. [Forwarding Props Using Rest Props](https://github.com/alialaa/svelte-course/tree/restprops)

**Section 4: Diving Deeper With a TODO List Component**

1. [#each Loop](https://github.com/alialaa/svelte-course/tree/todos-each-loop)
2. [Input Binding](https://github.com/alialaa/svelte-course/tree/input-binding)
3. [Updating Array](https://github.com/alialaa/svelte-course/tree/updating-todos-array)
4. [Binding Component Props](https://github.com/alialaa/svelte-course/tree/prop-binding)
5. [Dispatching Custom Events](https://github.com/alialaa/svelte-course/tree/custom-events)

**Section 5: **

**Section 6: **

**Section 7: **

**Section 8: **

**Section 9: **

**Section 10: SvelteKit Pages & Layout**

1. [Introduction to SvelteKit](https://svelte.dev/docs/kit/glossary)
2. [Creating Project Structure](https://svelte.dev/docs/kit/project-structure)
3. [Creating Routes](https://github.com/alialaa/sveltekit-course/tree/routing-basics)
4. [The $lib Folder Alias & Custom Aliases](https://github.com/alialaa/sveltekit-course/tree/organazing-components)
5. [Navigation Functions: goto(), beforeNavigate() & afterNavigate()](https://github.com/alialaa/sveltekit-course/tree/navigation-functions)

**Section 11: **

**Section 12: **

**Section 13: **

**Section 14: **

**Section 15: **

**Section 16: **

**Section 17: **
