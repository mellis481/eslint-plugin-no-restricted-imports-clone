# eslint-plugin-no-restricted-imports-clone

ESLint rule to allow for multiple severities to be used for no-restricted-imports.

### Background

Discussed in this issue: https://github.com/eslint/eslint/issues/14061

### Getting started

In your `.eslintrc.js` file:

- add `'no-restricted-imports-clone` to the `plugins` array.
- add the following the `rules` object:

```
    'no-restricted-imports': [
      'error',
      {
        name: 'someDependency',
        message: "Don't import someDependency.",
      },
    ],
    'no-restricted-imports-clone/no-restricted-imports-clone': [
      'warn',
      {
        name: 'anotherDependency',
        message: "You are encouraged to not import anotherDependency.",
      },
    ],
```
