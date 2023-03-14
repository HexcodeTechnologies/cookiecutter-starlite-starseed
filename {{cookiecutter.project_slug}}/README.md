<!-- markdownlint-disable -->
<p align="center">
  <img src="https://github.com/starlite-api/branding/blob/9ab099a2089219c07727baaa29f67e9474ff93c8/assets/Starlite%20Branding%20-%20SVG%20-%20Transparent/Logo%20-%20Banner%20-%20Inline%20-%20Light.svg#gh-light-mode-only" alt="Starlite Logo - Light" width="100%" height="auto" />
  <img src="https://github.com/starlite-api/branding/blob/9ab099a2089219c07727baaa29f67e9474ff93c8/assets/Starlite%20Branding%20-%20SVG%20-%20Transparent/Logo%20-%20Banner%20-%20Inline%20-%20Dark.svg#gh-dark-mode-only" alt="Starlite Logo - Dark" width="100%" height="auto" />
</p>
<!-- markdownlint-restore -->

<div align="center">

[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite-hello-world&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite-hello-world)
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite-hello-world&metric=coverage)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite-hello-world)
[![Technical Debt](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite-hello-world&metric=sqale_index)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite-hello-world)
[![Maintainability Rating](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite-hello-world&metric=sqale_rating)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite-hello-world)
[![Reliability Rating](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite-hello-world&metric=reliability_rating)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite-hello-world)
[![Vulnerabilities](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite-hello-world&metric=vulnerabilities)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite-hello-world)
[![Bugs](https://sonarcloud.io/api/project_badges/measure?project=starlite-api_starlite-hello-world&metric=bugs)](https://sonarcloud.io/summary/new_code?id=starlite-api_starlite-hello-world)

[![Discord](https://img.shields.io/discord/919193495116337154?color=202235&label=%20Discord&logo=discord)](https://discord.gg/X3FJqy8d2j) [![Matrix](https://img.shields.io/badge/%5Bm%5D%20Matrix-bridged-blue?color=202235)](https://matrix.to/#/#starlitespace:matrix.org) [![Reddit](https://img.shields.io/reddit/subreddit-subscribers/starlite?label=r%2FStarlite&logo=reddit)](https://reddit.com/r/starlite)

</div>

# starlite-hello-world

Minimum Starlite API Implementation.

`$ poetry install`

`$ poetry run uvicorn main:app --reload`

`$ curl localhost:8000/ -w "\n"`

## To use for Starlite development

If you want to use this app to test a local version of `Starlite`, the starlite dependency in
`pyroject.toml` to:

```toml
starlite = {path = "../starlite", develop = true}
```

This assumes that `Starlite` and this app exist in the same directory.

Run uvicorn with:

`$ poetry run uvicorn main:app --reload --reload-dir "../starlite/starlite"`

## Code Quality

After cloning:

`$ pre-commit install`

Run on all files:

`$ pre-commit run --all-files`

Run a specific hook:

`$ pre-commit run mypy --all-files`
