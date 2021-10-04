Project aiming to help reproduce the errors when setting up ESLint + Prettier with Svelte 3.

Plugins used:
- eslint-plugin-prettier
- eslint-plugin-svelte3
- prettier-plugin-svelte

To run (first, run `npm install`):

```
npm run dev
```

Then follow the link in terminal.

## Steps to reproduce the error

1. Run `npm install`;
2. Make sure you have ESLint and Prettier extensions configured in your editor;
3. Open this project;
4. Open `Counter.svelte`.

At the last step you should see an lint error as follows:

```
[Error - 11:54:15 PM] ESLint stack trace:
[Error - 11:54:15 PM] ParseError: Unexpected token
  1 | let count = 0;
  2 |
> 3 | {;}
    | ^
Occurred while linting /svelte-eslint-prettier-error/src/Counter.svelte:3
```