# @mfilin/prettier-config

Extendable prettier configuration from person who's lazy enough to pack single config as a npm package.
Comes with both prettier config and `.prettierignore`.

## Installation

```bash
npm i --save-dev @mfilin/prettier-config
```

## Configuration

There are multiple options. Note that you need only one of them, refer to [official
docs](https://prettier.io/docs/en/configuration)

In package.json:

```json
"prettier": "@mfilin/prettier-config"
```

In `.prettierrc`:

```json
"@mfilin/prettier-config"
```

## Extending .prettierignore

I'm not aware of a way to extend `.prettierignore` in a fancy way, but prettier can be run with `ignore-path` flag in
the CLI.

```bash
npx prettier . --write --ignore-path node_modules/@mfilin/prettier-config/.prettierignore
```
