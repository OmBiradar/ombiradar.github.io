---
layout: post
title: "RSTUF: Migrating to uv"
categories: RSTUF
---

## Motivation

`uv` is faster that `pip`.

## The Move

- Replace the files specific to `pipenv` like `Pipfile` with files
  specific to `uv` like `pyproject.toml`.
- Update testing
- Update CI
- Update `README.md`
