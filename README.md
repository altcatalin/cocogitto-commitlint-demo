# cocogitto-commitlint-demo

This is a demo of using [commitlint](https://commitlint.js.org/#/) as [pre-commit](https://pre-commit.com/) hook and [cocogitto/cocogitto-action](https://github.com/cocogitto/cocogitto-action) GitHub action.

## Development

```shell
pre-commit install --hook-type commit-msg
```

## Tests

1. default configuration
2. default configuration, `fix` commit type
3. default configuration, `feat` commit type
4. default configuration, `feat` commit type with `!` after type

Findings:

- cocogitto failing on first commit of type `feat`
- cocogitto it will never do an auto bump to the `1.0.0` version - see [cocogitto note](https://docs.cocogitto.io/guide/#auto-bump)
