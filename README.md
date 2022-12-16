# `@feedzai/prettier-config`

Feedzai's [Prettier](https://prettier.io/) configuration.

## Intro

Prettier is an opinionated code formatter. It enforces a consistent style by parsing your code and re-printing it with its own rules that take the maximum line length into account, wrapping code when necessary.

## Usage

First, install Prettier and `@feedzai/prettier-config` locally:

```bash
npm install --save-dev prettier @feedzai/prettier-config
```

or

```bash
yarn add --dev prettier @feedzai/prettier-config
```

or

```bash
pnpm add --save-dev prettier @feedzai/prettier-config
```

After that, edit the `package.json` file (as below) or one of the supported [configuration files](https://prettier.io/docs/en/configuration.html#sharing-configurations):

```json
{
  // ...
  "prettier": "@feedzai/prettier-config"
}
```

For a quick tour of how to use Prettier, check out the [Install page](https://prettier.io/docs/en/install.html) in the documentation.

## Development

After changes, sort the `package.json` file and run Prettier:

```bash
npx sort-package-json package.json
```

```bash
npx prettier --config ./index.json --write ./*.json
```
