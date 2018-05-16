# normalize.css without attribute selectors

> This is a fork of the famous normalize.css from Nicolas Gallagher and 
Jonathan Neal where all attribute selectors have been removed.

[![npm][npm-image]][npm-url] [![license][license-image]][license-url]
[![changelog][changelog-image]][changelog-url]


**NPM**

```sh
npm install --save normalize.css-without-attribute-selectors
```

## Why remove attribute selectors?

There is a huge performance bottleneck in Microsofts Internet Explorer 11 
when using attribute selectors. Rendering or styling of DOM elements takes up to
30-50 times longer when attributed selectors are involved. It's not only the 
usage of these selectors but there sole existance in a parsed CSS file or in a
`<style>` tag.

Alexei Antipov wrote an excellent article on 
[Medium.com](https://medium.com/@antipov.alexei/ie11-performance-bottleneck-de304569361d) 
where he figured out this IE11 issue.

## Usage

```css
@import 'node_modules/normalize.css-without-attribute-selectors/normalize.css';
```

or

```html
<link rel="stylesheet" href="node_modules/normalize.css-without-attribute-selectors/normalize.css">
```

## Credits

All credit should go to `normalize.css`. I just removed all attribute selectors. If you have questions about the source, check out the [original source](https://github.com/necolas/normalize.css/blame/master/normalize.css) and [this](https://github.com/necolas/normalize.css#extended-details-and-known-issues) for details.

## License

MIT


[changelog-image]: https://img.shields.io/badge/changelog-md-blue.svg?style=flat-square
[changelog-url]: CHANGELOG.md
[license-image]: https://img.shields.io/npm/l/normalize.css.svg?style=flat-square
[license-url]: LICENSE.md
[npm-image]: https://img.shields.io/npm/v/normalize.css.svg?style=flat-square
[npm-url]: https://www.npmjs.com/package/normalize.css
