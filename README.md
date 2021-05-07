# Feedzai prettier-config

## Intro

Prettier is an opinionated code formatter. It enforces a consistent style by parsing your code and re-printing it with its own rules that take the maximum line length into account, wrapping code when necessary.

## Install
First, install Prettier locally:

```bash
npm install --save-dev --save-exact prettier
```
or

```bash
yarn add --dev --exact prettier
```

Now, copy one of prettier file (can be .prettierrc, .prettier.yaml or prettier.config.js) inside your project.

After this step, watch the package.json inside your project, there will be more information about how to run prettier in your project. As a example we can run like example in below:

Now, format all files with Prettier:

```bash
npx prettier --write .
```

or

```bash
yarn prettier --write .
```

`prettier --write .` is great for formatting everything, but for a big project it might take a little while. You may run `prettier --write app/` to format a certain directory, or `prettier --write app/components/Button.js` to format a certain file. Or use a _glob_ like `prettier --write "app/**/*.test.js"` to format all tests in a directory (see [fast-glob](https://github.com/mrmlnc/fast-glob#pattern-syntax) for supported glob syntax).

If you have a CI setup, run the following as part of it to make sure that everyone runs Prettier. This avoids merge conflicts and other collaboration issues!

```bash
npx prettier --check .
```

`--check` is like `--write`, but only checks that files are already formatted, rather than overwriting them. `prettier --write` and `prettier --check` are the most common ways to run Prettier.

## Set up your editor

Formatting from the command line is a good way to get started, but you get the most from Prettier by running it from your editor, either via a keyboard shortcut or automatically whenever you save a file. When a line has gotten so long while coding that it won’t fit your screen, just hit a key and watch it magically be wrapped into multiple lines! Or when you paste some code and the indentation gets all messed up, let Prettier fix it up for you without leaving your editor.

## ESLint (and other linters)

If you use ESLint, install [eslint-config-prettier](https://github.com/prettier/eslint-config-prettier#installation) to make ESLint and Prettier play nice with each other. It turns off all ESLint rules that are unnecessary or might conflict with Prettier. There’s a similar config for Stylelint: [stylelint-config-prettier](https://github.com/prettier/stylelint-config-prettier)

## References
[Prettier](https://prettier.io)
[Editor Integration](https://prettier.io/docs/en/editors.html)
[How to set options in Prettier](https://prettier.io/docs/en/options.html)

Ticket reference: IT-26969
