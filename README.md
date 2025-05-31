# Novo Elements: Angular to Vue 3 Porting Guide (Windsurf Rule)

## Purpose

We are porting Novo Elements from Angular components to Vue 3 components. This is a foundational change intended to modernize the codebase, improve maintainability, and leverage Vue’s reactive and composition-based architecture.

## Scope

- All new UI components should be written in Vue 3.
- Legacy Angular components will be phased out as their Vue equivalents are completed.
- The goal is feature parity with the Angular components, but improvements and simplifications are encouraged where appropriate.

## Best Practices & Guidelines

### 1. Component Structure

- Use the `<script setup>` syntax for new Vue components.
- Prefer Composition API over Options API for new code.
- Organize components in a flat structure under `src/components`, using PascalCase for filenames.

### 2. State Management

- Use Vue’s built-in reactivity for local state.
- For shared state, prefer Pinia or Vue’s provide/inject over Vuex (if starting fresh).

### 3. Styling

- Use scoped CSS or CSS Modules.
- Prefer Tailwind CSS or a utility-first approach if the project allows.
- Avoid Angular-specific styling or encapsulation patterns.

### 4. Testing

- Write unit tests with Vitest or Jest.
- Use Vue Test Utils for component testing.

### 5. Migration Process

- When porting a component, create a matching Vue 3 version in `src/components`.
- Ensure feature parity; document any intentional changes.
- Write migration notes in the component’s README if there are API or UX differences.

### 6. Code Quality

- Follow the project’s ESLint and Prettier rules.
- Use TypeScript for all new code.
- Document public props, emits, and slots in JSDoc or markdown.

## References


## Dependencies

- [NodeJS v18.3+](https://nodejs.org/en/)

## Quick Start

    # Clone the project
    git clone git@github.com:bullhorn/novo-elements.git

    # Change directory
    cd novo-elements

    # Install
    npm install

    # Start (you will need two terminals)
    npm run build (builds the library, alternatively you can use npm run build:watch for live-reload)
    npm start (starts the demo)

    # Access the Demo in your browser at
    http://localhost:4200/

## Integrating into a project

    # Install the module from NPM
    npm install --save novo-elements

Depending on what system you are using (SystemJS, Webpack, etc..) the setup will vary.

If using SCSS/SASS you will need to include the following includes: `node_modules/novo-elements/lib`.

## Building Examples

> All examples can be added to the appropriate directory in the `novo-examples` project. Each markdown file will be converted to a demo page and a route will automatically be added to the demo. You can import any example project by using the angular selector, or inject it using the `code-example` tag, ie. `<code-example example="demo-name"></code-example>`.

    # Compile markdown, generate routes, and AOT build the project
    npm run build:examples

    # Automatically rebuild changes to the examples project
    npm run build:examples:watch

## Customizing Labels

With Novo Elements there are a few hard-coded labels throughout the library. To override these labels with your own, you will simply extend the `NovoLabelService` and override any labels that you wish.

To make Angular use this new class over the default one you can provide in the bootstrapping of your application as a provider.

```ts
{ provide: NovoLabelService, useClass: MyLabelService }
```

To use the default labels, you will need to provide the `NOVO_ELEMENTS_LABELS_PROVIDERS` via

```ts
import {NOVO_ELEMENTS_LABELS_PROVIDERS} from 'novo-elements';
bootstrap(MyApp [..NOVO_ELEMENTS_LABELS_PROVIDERS]);
```

## Contribute

There are many ways to **[contribute](https://github.com/bullhorn/novo-elements/blob/master/CONTRIBUTING.md)** to our OpenSource projects.

- **[Submit bugs](https://github.com/bullhorn/novo-elements/issues)** and help us verify fixes as they are checked in.
- Review **[source code changes](https://github.com/bullhorn/novo-elements/pulls)**.
- **[Contribute bug fixes](https://github.com/bullhorn/novo-elements/blob/master/CONTRIBUTING.md)**.

> TL;DR: Fork this repository, make any required change and then submit a PR :)

# License

Copyright (c) forever [Bullhorn](http://www.bullhorn.com).

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
