---
layout: post
title: "RSTUF: Migrating to uv"
categories: python
---

## Motivation

`uv` is faster that `pip`.

## The Move

Currently RSTUF uses `pipenv` which is a combination of `pip`
and `virtualenv`. `uv` does the same functions of `pipenv`,
As `uv` is faster than `pip`, it's a good replacement for `pipenv`.

The move would include removal of `Pipfile` and replacing it with
`pyproject.toml` which `uv` uses. This needs to be done carefully
to ensure the packages and their versions are translated exactly
from `Pipfile` to `pyproject.toml`.

Other workflows that use `pipenv` need to be changed to use `uv`.
