# mode-compile.el

This is mode-compile.el v2.29.1 (obtained from
https://gist.githubusercontent.com/yaa/0f02f59399ee6d08c5b72b504318d2d5/raw/82681792a52fac1dee0507da6978c8184f8f985d/mode-compile.el)
and modernised so as to be usable with emacs 27 and later (but also
works with emacs 26; don't know about anything earlier).

The primary reason for doing this was for use with perl. Only minimal
testing had been done, and only with perl.

## specific errors corrected

* `cl` is deprecated - use `cl-lib` instead
* `eval-when` is undefined - use `cl-eval-when` instead
* `(lambda (x) ...)` quoted with `'` rather than with `#'` - replace `'(lambda` with `#'(lambda`
* old-style backquotes detected - replace ```(` (foo (, bar)))``` with ``` `(foo ,bar)```

## Changes

3.01 20212705
  - add myself as maintainer
  - add this changelog

3.00 20210401
  - use "modern" emacs
