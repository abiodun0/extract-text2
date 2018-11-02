# Webpack blocks - Extract text plugin for Webpack 2

[![JavaScript Style Guide](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com/)

This is the block providing configuration for the [extract-text-webpack-plugin](https://github.com/webpack/extract-text-webpack-plugin). Use it to extract SCSS styles out of the bundle and into a separate CSS file.

This is based on [webpack-blocks](https://github.com/andywer/webpack-blocks)


## Usage

```js
const { createConfig } = require('@webpack-blocks/webpack')
const extractText = require('@thezebra/extract-text2')

module.exports = createConfig([
  ...,
    extractText(`css/${fileName}.css`, 'text/x-sass'),   // or just `extractText()`
])
```

to include postcss-loader, pass a third paramter
```js
  extractText(`css/${fileName}.css`, 'text/x-sass', true),
```


## Webpack blocks

Check out the

👉 [Main Documentation](https://github.com/andywer/webpack-blocks)

Released under the terms of the MIT license.
