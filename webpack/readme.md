# webpack

## webpack 1:
- create bundle file
cli: 
$ webpack ./entry.js bundle.js
source: https://webpack.github.io/docs/tutorials/getting-started/

## webpack 2:
- create bundle file from the second file
cli: 
$ webpack ./entry.js bundle.js
source: https://webpack.github.io/docs/tutorials/getting-started/

## webpack 3:
- We want to add a CSS file to our application.
- webpack can only handle JavaScript natively, so we need the css-loader to process CSS files. We also need the style-loader to apply the styles in the CSS file.
- Run npm install css-loader style-loader to install the loaders. (They need to be installed locally, without -g) This will create a node_modules folder for you, in which the loaders will live.
cli: 
$ webpack ./entry.js bundle.js
source: https://webpack.github.io/docs/tutorials/getting-started/
ref: https://webpack.js.org/guides/migrating/#automatic-loader-module-name-extension-removed

## webpack 4:
- binding loaders
cli:
webpack ./entry.js bundle.js --module-bind 'css=style-loader!css-loader'
source: https://webpack.github.io/docs/tutorials/getting-started/
ref: https://webpack.js.org/guides/

## webpack 5:
- config file
- watch mode: When using watch mode, webpack installs file watchers to all files, which were used in the compilation process. If any change is detected, it’ll run the compilation again. When caching is enabled, webpack keeps each module in memory and will reuse it if it isn’t changed.
cli:
webpack --watch
source: https://webpack.github.io/docs/tutorials/getting-started/
