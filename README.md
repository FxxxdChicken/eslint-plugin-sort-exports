# eslint-plugin-sort-exports

Sort export declarations in modules, similarly to [sort-imports](https://eslint.org/docs/rules/sort-imports)

## Installation

First install [ESLint](https://www.eslint.org)

```
yarn add -d eslint
```

Then install `eslint-plugin-sort-exports`

```
yarn add --dev https://github.com/FxxxdChicken/eslint-plugin-sort-exports
// or
npm i -D https://github.com/FxxxdChicken/eslint-plugin-sort-exports
```

**Note:** If you installed ESLint globally, you must also install `eslint-plugin-sort-exports` globally.

## Usage

Add `sort-exports` to the plugins section of your `.eslintrc` and configure the rule under the `rules` section.

```
{
    "plugins": ["sort-exports"],
    "rules": {
        "sort-exports/sort-exports": ["error", {"sortDir": "asc"}]
    }
}
```

## Supported rules

```
sort-exports
```

## Configuration

```
{
    "sort-exports/sort-exports": [
        "error",
        { sortDir: "asc", ignoreCase: true }
    ]
}
```

Options can be any of the following properties:

- `sortDir`: Can be either `asc` (default) or `desc` signifying ascending or descending sort order, respectively.
- `ignoreCase`: If true, sorting is case-insensitive.
