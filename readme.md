# Modular Type Scale

A basic Sass build to handle scaling type, based on methods in Matej Latin's _Better Web Typography for a Better Web_.

## Build
Compiled CSS is included in repo. If testing changes such as a different modular scale, run a simple sass command to rebuild:
`sass src/sass/style.css build/css/style.css`

## Concepts
Modular scale allows for a math-based typographic scale to determine various font sizes based on the supplied base size and scale. The included sass uses a power function `pow()` to calculate the various sizes needed for the scale, and a modular scale function `ms()` to supply each of these computed sizes to elements on demand. There are also line-height and margin mixins to properly calculate values against the supplied base and scale.

## Grid (optional)
To turn off the scale grid (enabled by default), simply remove the `grid` and/or `double-grid` classes on the `<html>` element.