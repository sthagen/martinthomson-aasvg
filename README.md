# aasvg

Convert ASCII art diagrams into SVG.

This is inspired by [goat](https://github.com/blampe/goat) but rather than a
reimplementation, this code uses the original
[markdeep](https://casual-effects.com/markdeep/) code.

## Usage

Install with `npm install -g aasvg`.

Feed `aasvg` an image and it will write an SVG.  For example:

```
$ aasvg < example.txt > example.svg
```

<!-- generate this with the ~~backdrop option to avoid it looking terrible
     when shown on GitHub in dark mode -->
![example](./example.svg)

## Significant Changes

By default, this does not place text characters on a grid one-by-one.  This
improves accessibility at the cost of having characters less precisely placed.
The `--text-grid` option can be used to enable precise placement.
