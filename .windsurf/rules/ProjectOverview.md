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

### Migration Progress Tracking Rule

- **Whenever a component is ported, or its migration status changes, you must update [`TODO.md`](../../TODO.md) to reflect the new status. This ensures migration progress is always up to date and visible to all contributors.**

### 6. Code Quality

- Follow the project’s ESLint and Prettier rules.
- Use TypeScript for all new code.
- Document public props, emits, and slots in JSDoc or markdown.

## References

- [Vue 3 Docs](https://vuejs.org/)
- [Pinia Docs](https://pinia.vuejs.org/)
- [Vue Test Utils](https://test-utils.vuejs.org/)
