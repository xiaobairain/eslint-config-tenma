# eslint-config-tenma


## Installation

```
$ npm install --save-dev eslint eslint-plugin-react eslint-config-tenma
```

## Usage

Once the `eslint-config-tenma` package is installed, you can use it by specifying `tenma` in the [`extends`](http://eslint.org/docs/user-guide/configuring#extending-configuration-files) section of your [ESLint configuration](http://eslint.org/docs/user-guide/configuring).

```js
{
  "extends": "tenma",
  "rules": {
    // Additional, per-project rules...
  }
}
```

### Using the `tenma` config with `eslint:recommended`

There are several rules in the [`eslint:recommended` ruleset](http://eslint.org/docs/rules/) that TENMA style is not opinionated about that you might want to enforce in your project.

To use TENMA style in conjunction with ESLint's recommended rule set, extend them both, making sure to list `tenma` last:

```js
{
  "extends": ["eslint:recommended", "plugin:react/recommended", "tenma"],
  "rules": {
    // Additional, per-project rules...
  }
}
```

## License

ISC
