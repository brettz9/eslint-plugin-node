# eslint-plugin-node

[![npm version](https://img.shields.io/npm/v/eslint-plugin-node.svg)](https://www.npmjs.com/package/eslint-plugin-node)
[![Downloads/month](https://img.shields.io/npm/dm/eslint-plugin-node.svg)](http://www.npmtrends.com/eslint-plugin-node)
[![Build Status](https://travis-ci.org/mysticatea/eslint-plugin-node.svg?branch=master)](https://travis-ci.org/mysticatea/eslint-plugin-node)
[![Coverage Status](https://codecov.io/gh/mysticatea/eslint-plugin-node/branch/master/graph/badge.svg)](https://codecov.io/gh/mysticatea/eslint-plugin-node)
[![Dependency Status](https://david-dm.org/mysticatea/eslint-plugin-node.svg)](https://david-dm.org/mysticatea/eslint-plugin-node)

Additional ESLint's rules for Node.js

## 💿 Install & Usage

```
$ npm install --save-dev eslint eslint-plugin-node
```

- Requires Node.js `^4.0.0 || >=6.0.0`
- Requires ESLint `>=3.1.0`

**Note:** It recommends a use of [the "engines" field of package.json](https://docs.npmjs.com/files/package.json#engines). The "engines" field is used by [no-unsupported-features](docs/rules/no-unsupported-features.md) rule.

**.eslintrc.json** (An example)

```json
{
    "extends": ["eslint:recommended", "plugin:node/recommended"],
    "rules": {
        "node/exports-style": ["error", "module.exports"]
    }
}
```

**package.json** (An example)

```json
{
    "name": "your-module",
    "version": "1.0.0",
    "engines": {
        "node": ">=4.0.0"
    }
}
```

## 📖 Rules

- ⭐️ - the mark of recommended rules.
- ✒️ - the mark of fixable rules.

<!--RULES_TABLE_START-->
### Possible Errors

| Rule ID | Description |    |
|:--------|:------------|:--:|
| [node/no-extraneous-import](./docs/rules/no-extraneous-import.md) | disallow `import` declarations of extraneous packages |  |
| [node/no-extraneous-require](./docs/rules/no-extraneous-require.md) | disallow `require()` expressions of extraneous packages | ⭐️ |
| [node/no-missing-import](./docs/rules/no-missing-import.md) | disallow `import` declarations of missing files |  |
| [node/no-missing-require](./docs/rules/no-missing-require.md) | disallow `require()` expressions of missing files | ⭐️ |
| [node/no-unpublished-bin](./docs/rules/no-unpublished-bin.md) | disallow 'bin' files which are ignored by npm | ⭐️ |
| [node/no-unpublished-import](./docs/rules/no-unpublished-import.md) | disallow `import` declarations of private things |  |
| [node/no-unpublished-require](./docs/rules/no-unpublished-require.md) | disallow `require()` expressions of private things | ⭐️ |
| [node/no-unsupported-features/assert](./docs/rules/no-unsupported-features/assert.md) | disallow unsupported `assert` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/async_hooks](./docs/rules/no-unsupported-features/async_hooks.md) | disallow unsupported `async_hooks` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/buffer](./docs/rules/no-unsupported-features/buffer.md) | disallow unsupported `buffer` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/child_process](./docs/rules/no-unsupported-features/child_process.md) | disallow unsupported `child_process` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/console](./docs/rules/no-unsupported-features/console.md) | disallow unsupported `console` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/crypto](./docs/rules/no-unsupported-features/crypto.md) | disallow unsupported `crypto` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/dns](./docs/rules/no-unsupported-features/dns.md) | disallow unsupported `dns` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/ecma](./docs/rules/no-unsupported-features/ecma.md) | disallow unsupported ECMAScript features on the specified version | ⭐️ |
| [node/no-unsupported-features/fs](./docs/rules/no-unsupported-features/fs.md) | disallow unsupported `fs` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/http2](./docs/rules/no-unsupported-features/http2.md) | disallow unsupported `http2` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/inspector](./docs/rules/no-unsupported-features/inspector.md) | disallow unsupported `inspector` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/module](./docs/rules/no-unsupported-features/module.md) | disallow unsupported `module` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/os](./docs/rules/no-unsupported-features/os.md) | disallow unsupported `os` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/path](./docs/rules/no-unsupported-features/path.md) | disallow unsupported `path` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/perf_hooks](./docs/rules/no-unsupported-features/perf_hooks.md) | disallow unsupported `perf_hooks` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/process](./docs/rules/no-unsupported-features/process.md) | disallow unsupported `process` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/stream](./docs/rules/no-unsupported-features/stream.md) | disallow unsupported `stream` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/trace_events](./docs/rules/no-unsupported-features/trace_events.md) | disallow unsupported `trace_events` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/url](./docs/rules/no-unsupported-features/url.md) | disallow unsupported `url` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/util](./docs/rules/no-unsupported-features/util.md) | disallow unsupported `util` APIs on the specified version | ⭐️ |
| [node/no-unsupported-features/v8](./docs/rules/no-unsupported-features/v8.md) | disallow unsupported `v8` APIs on the specified version | ⭐️ |
| [node/process-exit-as-throw](./docs/rules/process-exit-as-throw.md) | make `process.exit()` expressions the same code path as `throw` | ⭐️ |
| [node/shebang](./docs/rules/shebang.md) | enforce the correct usage of shebang | ⭐️✒️ |

### Best Practices

| Rule ID | Description |    |
|:--------|:------------|:--:|
| [node/no-deprecated-api](./docs/rules/no-deprecated-api.md) | disallow deprecated APIs | ⭐️ |

### Stylistic Issues

| Rule ID | Description |    |
|:--------|:------------|:--:|
| [node/exports-style](./docs/rules/exports-style.md) | enforce either `module.exports` or `exports` |  |

<!--RULES_TABLE_END-->

## 🔧 Configs

This plugin provides `plugin:node/recommended` preset config.
This preset config:

- enables the environment of ES2015 (ES6) and Node.js.
- enables rules which are given :star: in the above table.
- enables [no-process-exit](http://eslint.org/docs/rules/no-process-exit) rule because [the official document](https://nodejs.org/api/process.html#process_process_exit_code) does not recommend a use of `process.exit()`.
- adds `{ecmaVersion: 2018}` into `parserOptions`.
- adds `Atomics` and `SharedArrayBuffer` into `globals`.

## 👫 FAQ

- Q: The `no-missing-import` / `no-missing-require` rules don't work with nested folders in SublimeLinter-eslint
- A: See [context.getFilename() in rule returns relative path](https://github.com/roadhump/SublimeLinter-eslint#contextgetfilename-in-rule-returns-relative-path) in the SublimeLinter-eslint FAQ.

## 🚥 Semantic Versioning Policy

`eslint-plugin-node` follows [semantic versioning](http://semver.org/) and [ESLint's Semantic Versioning Policy](https://github.com/eslint/eslint#semantic-versioning-policy).

- Patch release (intended to not break your lint build)
    - A bug fix in a rule that results in it reporting fewer errors.
    - Improvements to documentation.
    - Non-user-facing changes such as refactoring code, adding, deleting, or modifying tests, and increasing test coverage.
    - Re-releasing after a failed release (i.e., publishing a release that doesn't work for anyone).
- Minor release (might break your lint build)
    - A bug fix in a rule that results in it reporting more errors.
    - A new rule is created.
    - A new option to an existing rule is created.
    - An existing rule is deprecated.
- Major release (likely to break your lint build)
    - A support for old Node version is dropped.
    - A support for old ESLint version is dropped.
    - An existing rule is changed in it reporting more errors.
    - An existing rule is removed.
    - An existing option of a rule is removed.
    - An existing config is updated.

## 📰 Changelog

- [GitHub Releases](https://github.com/mysticatea/eslint-plugin-node/releases)

## 💎 Contributing

Welcome contributing!

Please use GitHub's Issues/PRs.

### Development Tools

- `npm test` runs tests and measures coverage.
- `npm run coverage` shows the coverage result of `npm test` command.
- `npm run clean` removes the coverage result of `npm test` command.
