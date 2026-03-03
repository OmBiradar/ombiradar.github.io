---
layout: post
title: "Rust: Tokio crate"
date: 2026-03-03 15:30:00 +0530
categories: rust async tokio
---

#### What is Tokio?

It's a helper.

It helps to run `async` jobs in rust.

<hr>

#### Why use tokio?

Without `tokio`:
* handle all multi threading or `async` operations manually, like in `C++`.

With `tokio`: it provides
* task scheduler (multi thread and single thread)
* async input/output (TCP, UDP, files...)
* timers, delays, intervals
* spaw thousands of lightweight tasks

Kind of similar to `go routines`

<hr>

#### References

* [rust docs](https://docs.rs/tokio/latest/tokio/)

<hr>

#### Next steps

Trying to build projects using `tokio` for clearer understanding.

Stay tuned.
