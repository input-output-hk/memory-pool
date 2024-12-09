# `memory-pool`

Thread-safe lock-free memory pool manager.

## Overview

Memory management utility that allows allocating large chunks of memory at once while
using it at a fine grain smaller block level. There is a restriction on the blocks of
memory to having the same size in a single pool.

This package was designed for Cardano cryptocurrency, but it is a general purpose Haskell
tool. The particular use cases in Cardano is to allocate one large page of memlocked
memory using libsodium and treat it as many smaller regions for secure storage and cleanup
of private keys.

## Status

| Github Actions | Coveralls | Hackage | Nightly | LTS |
|:--------------:|:---------:|:-------:|:-------:|:---:|
| [![Build Status][GA-badge]][GA-link] | [![Coverage Status][Coveralls-badge]][Coveralls-link] | [![Hackage][Hackage-badge]][Hackage-link] | [![Nightly][Nightly-badge]][Nightly-link] | [![LTS][LTS-badge]][LTS-link]

[GA-badge]: https://github.com/input-output-hk/memory-pool/workflows/CI/badge.svg
[GA-link]: https://github.com/input-output-hk/memory-pool/actions
[Coveralls-badge]: https://coveralls.io/repos/github/input-output-hk/memory-pool/badge.svg?branch=master
[Coveralls-link]: https://coveralls.io/github/input-output-hk/memory-pool?branch=master
[Hackage-badge]: https://img.shields.io/hackage/v/memory-pool.svg
[Hackage-link]: https://hackage.haskell.org/package/memory-pool
[Nightly-badge]: https://www.stackage.org/package/memory-pool/badge/nightly
[Nightly-link]: https://www.stackage.org/nightly/package/memory-pool
[LTS-badge]: https://www.stackage.org/package/memory-pool/badge/lts
[LTS-link]: https://www.stackage.org/lts/package/memory-pool
