---
title: "Use in Projects"
linkTitle: "Use in Projects"
weight: 10
description: >
  Learn how to install Rosely, integrate the palettes and use the colors in your own projects.
---

Rosely comes in many formats to cover a wide range of project types and tech stacks.
Its [colors and palettes](/docs/colours-and-palettes/) have especially been designed for UI elements and code syntax highlighting often found in projects build with web technologies like websites.

## Installation

Since Rosely is heavily used in web technology based projects, its main installation method is therefore [**npm**][npm], the [Node.js][] package manager.

Install and add it as production dependency by running `npm` from the command line:

```sh
npm install --save rosely
```

If you're using [**yarn**][yarn] instead of `npm` run the following command:

```sh
yarn add rosely
```

### From Source

If you'd like to install Rosely without `npm` or `yarn` you can use it from source by either [downloading individual source files][gh-tree-src] or [cloning the repository][gh].

## Usage

Next to the available <Link to={ROUTE_DOCS_SWATCHES}>color swatches</Link> for your favorite applications, Rosely is available in many module formats for various CSS [preprocessors][wiki-preproc].

### Sass

[Sass][] is a mature, stable, and powerful professional grade CSS preprocessor and extension language.
Rosely is available as [SCSS syntax module][sass-docs-scss] that can be imported using the [`@import`][sass-docs-import] @-rule that extends the [default CSS `@import`][mdn-css-@import] @-rule:

```scss
@import "node_modules/rosely/src/sass/rosely.scss";

body {
  background-color: $rosely0;
  color: $rosely8;
}
```

Please see the official [Sass syntax][sass-docs-syntax] documentation for more details about differences to the [indented Sass syntax][sass-docs-syntax-indented].

The [Sass module][gh-tree-sass] provides all <Link to={ROUTE_DOCS_COLOR_AND_PALETTES}>Rosely colors</Link> as [Sass variables][sass-docs-vars] from `$rosely0` to `$rosely15`.

### Less

[Less][] is a dynamic CSS preprocessor and extension language that was influenced by [Sass][] and has influenced the newer [SCSS syntax][sass-docs-scss].
Rosely can be [imported as Less module][less-docs-importing] using the [`@import`][sass-docs-import] @-rule that extends the [default CSS `@import`][mdn-css-@import] @-rule:

```less
@import "node_modules/rosely/src/rosely.less";

body {
  background-color: @rosely0;
  color: @rosely8;
}
```

The [Less module][gh-tree-less] provides all <Link to={ROUTE_DOCS_COLOR_AND_PALETTES}>Rosely colors</Link> as [Less variables][less-docs-vars] from `@rosely0` to `@rosely15`.

### Stylus

[Stylus][] is a dynamic CSS preprocessor and extension language that was influenced by [Sass][] and [Less][].
Rosely can be imported as [Stylus module][stylus-docs-import] using the `@import` @-rule, which extends the [default CSS `@import`][mdn-css-@import] @-rule, or the Stylus specific [`@require`][stylus-docs-import-req] @-rule:

```stylus
@import "node_modules/rosely/src/rosely.styl";

body {
  background-color: @rosely0;
  color: @rosely8;
}
```

The [Stylus module][gh-tree-stylus] provides all <Link to={ROUTE_DOCS_COLOR_AND_PALETTES}>Rosely colors</Link> as [Stylus variables][stylus-docs-vars] from `@rosely0` to `@rosely15`.

### CSS

The [CSS specification][w3-css-spec-vars] supports the definition of **custom properties**, often referred to as **CSS variables**, that contain specific values to be reused throughout a document.
They are set using custom property notation (e.g. `--rosely8: #88c0d0;`) and are accessed using the CSS [`var()`][mdn-css-func-var] function (e.g. `color: var(--rosely8);`).

Rosely can be imported as [CSS module][stylus-docs-import] using the [CSS `@import`][mdn-css-@import] @-rule:

```css
@import "node_modules/rosely/src/rosely.css";

body {
  background-color: var(--rosely0);
  color: var(--rosely8);
}
```

If you're using the [PostCSS][] plugin [postcss-import][gh-postcss-import], Rosely can be simply imported like any JavaScript module:

```css
@import "rosely";
```

The [CSS module][gh-tree-css] provides all <Link to={ROUTE_DOCS_COLOR_AND_PALETTES}>Rosely colors</Link> as variables `--rosely0` to `--rosely15` nested inside the `:root` element selector.

## Source Code Documentation

The Sass module is documented using the [SassDoc][] comment syntax, a documentation system to build pretty and powerful docs from Sass files, while the Less and Stylus modules are documented using the [KSS][] comment syntax, a documentation syntax that is human readable, but just structured enough to be machine parsable.

Both SassDoc and KSS can be used to generate a static, fully styled HTML document from the source code. Please see the [official SassDoc documentation on how to get started][sassdoc-docs-start] and the [official KSS documentation on how to create styleguides][kss-docs-styleguides] for more details.

[gh-postcss-import]: https://github.com/postcss/postcss-import
[gh-tree-css]: https://github.com/hellotham/rosely/blob/develop/src/rosely.css
[gh-tree-less]: https://github.com/hellotham/rosely/blob/develop/src/rosely.less
[gh-tree-sass]: https://github.com/hellotham/rosely/blob/develop/src/rosely.scss
[gh-tree-src]: https://github.com/hellotham/rosely/tree/develop/src
[gh-tree-stylus]: https://github.com/hellotham/rosely/blob/develop/src/rosely.styl
[gh]: https://github.com/hellotham/rosely
[kss-docs-styleguides]: http://warpspire.com/kss/styleguides
[kss]: https://warpspire.com/kss
[less-docs-import-rule]: http://lesscss.org/features/#import-atrules-feature
[less-docs-importing]: http://lesscss.org/#importing
[less-docs-vars]: http://lesscss.org/features/#variables-feature
[less]: http://lesscss.org
[mdn-css-@import]: https://developer.mozilla.org/en-US/docs/Web/CSS/@import
[mdn-css-func-var]: https://developer.mozilla.org/en-US/docs/Web/CSS/var
[node.js]: https://nodejs.org
[npm]: https://www.npmjs.com
[postcss]: https://postcss.org
[sass-docs-import]: https://sass-lang.com/documentation/file.SASS_REFERENCE#import
[sass-docs-scss]: https://sass-lang.com/documentation/file.SCSS_FOR_SASS_USERS
[sass-docs-syntax-indented]: https://sass-lang.com/documentation/file.INDENTED_SYNTAX
[sass-docs-syntax]: https://sass-lang.com/documentation/file.SASS_REFERENCE#syntax
[sass-docs-vars]: https://sass-lang.com/documentation/file.SASS_REFERENCE#variables_
[sass]: https://sass-lang.com
[sassdoc-docs-start]: http://sassdoc.com/getting-started
[sassdoc]: http://sassdoc.com
[stylus-docs-import-req]: http://stylus-lang.com/docs/import#require
[stylus-docs-import]: http://stylus-lang.com/docs/import
[stylus-docs-vars]: http://stylus-lang.com/docs/variables
[stylus]: http://stylus-lang.com
[w3-css-spec-vars]: https://www.w3.org/TR/css-variables
[wiki-preproc]: https://en.wikipedia.org/wiki/Preprocessor
[yarn]: https://yarnpkg.com