# Gemma
[![npm-version](https://img.shields.io/npm/v/gemma.svg?style=flat)](https://www.npmjs.com/package/gemma)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](https://github.com/feross/standard)

## Tightly focused, highly composable CSS
Built for performance, maintenance, and (re)usability, Gemma is a collection of foundational styles and classes for creating beautifully simple, highly effective CSS.

It is currently in initial development and is _not_ ready for use yet. Stay tuned for updates and proper documentation.

## Philosophy
Gemma’s philosophical approach to CSS favours:

- mobile-first, lightweight styles
- responsive design as a default
- forming both basic and more nuanced components from independent, highly recombinable pieces (think Lego!)
- designing systems that are easy for developers and designers to learn and use
- delivering the smallest amount of CSS possible to devices, browsers, and users

Architectural and technical details can be found in [the source files readme](https://github.com/colepeters/gemma/tree/master/src).

## Usage
Gemma is not ready for production usage yet, though I have started using development builds on [my personal website](https://colepeters.com) and the [First Things First 2014 website](http://firstthingsfirst2014.org). Production-ready builds are still a couple minor version numbers away. Hold tight.

In the mean time, you can check the pre-release updates on [the releases page](https://github.com/colepeters/gemma/releases).

## Development
Gemma is under active development and is not considered ready for production usage yet. Contributions may be considered but given that critical development is still being defined, it may be a bit soon for PRs. With that said, to work on Gemma:

1. Clone the latest master branch of the repository (`git clone https://github.com/colepeters/gemma.git`)
2. `cd` to the repository and install dependencies via npm (`cd gemma && npm i`)

Development tasks are currently managed with Gulp via npm scripts:

### `npm run lint`
Gemma ships with a [linting configuration](https://github.com/colepeters/gemma/blob/master/stylelintrc.json) which is passed to [Stylelint](https://github.com/stylelint/stylelint). The lint task will examine all CSS files in the source directory, and output any linting errors to the command line via [postcss-reporter](https://github.com/postcss/postcss-reporter).

### `npm run compile`
Passes all source CSS files to [cssnext](https://github.com/cssnext/cssnext), via [gulp-postcss](https://github.com/postcss/gulp-postcss). This transforms source CSS custom properties to their computed values and minifies the output, resulting in a `gemma.min.css` file.

More development tasks (continuous compilation, watchers, etc) will be integrated shortly.

## Inspiration and motivation
Gemma is evolutionary, not revolutionary. Its philosophical and stylistic leanings have been heavily influenced by the following projects:

- [BassCSS](http://basscss.com)
- [Tachyons](http://tachyons.io)
- [OOCSS](https://github.com/stubbornella/oocss)
- [ITCSS](https://twitter.com/itcss_io)

and the following people:

- [@jxnblk](http://jxnblk.com)
- [@mrmrs](http://mrmrs.io)
- [@stubbornella](http://www.stubbornella.org/content/)
- [@necolas](http://nicolasgallagher.com/)
- [@csswizardry](http://csswizardry.com/)

(and likely more whom I’ve forgotten to mention).

* * *

_A gemma (/ˈdʒɛmə/ with a soft "g", as in "general") is a single cell, or a mass of cells, that detaches from the parent and develops into a new individual._
