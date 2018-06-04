[![Hackage](https://img.shields.io/hackage/v/ghcjs-base-stub.svg)](https://hackage.haskell.org/package/ghcjs-base-stub)
[![Build Status](https://secure.travis-ci.org/louispan/ghcjs-base-stub.png?branch=master)](http://travis-ci.org/louispan/ghcjs-base-stub)

Fake stubs for GHCJS base to allow GHCJS projects to be compiled using GHC.
This also allows developing under intero, and generating haddocks.

Usage:

Add the following to GHCJS project's cabal.
```
  if impl(ghcjs)
    build-depends: ghcjs-base
  if !impl(ghcjs)
    build-depends: ghcjs-base-stub
```

# Changelog

* 0.2.0.0
  - Added Semigroup instance to JSString for ghc 8.4.1 and base 4.11.0

* 0.1.0.4
  - Added Javascript.Web.Location

* 0.1.0.3
  - Added Javascript.Web.Storage

* 0.1.0.2
  - Added JavaScript.Cast
  - Added Marshall and Callbacks

* 0.1.0.0
  - Initial version with a subset of ghcjs base
