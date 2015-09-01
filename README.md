# admin-config [![Build Status](https://travis-ci.org/marmelab/admin-config.svg?branch=master)](https://travis-ci.org/marmelab/admin-config)

Common files used in both [ng-admin](https://github.com/marmelab/ng-admin) and [react-admin](https://github.com/marmelab/react-admin).

## Installation

```sh
make install
```

## Including In Another Library

Require whatever class you need directly.

```js
// es5
var NumberField = require('admin-config/lib/Field/NumberField');
// es6
import NumberField from "admin-config/lib/Field/NumberField";
```

Admin-config is written in ES6. You'll need a transpiler to use any of the classes (we recommend [Webpack](http://webpack.github.io/), using, for instance, [babel](https://babeljs.io/) to convert it to ES5. Here is an example Webpack configuration for that:

```js
module.exports = {
    // ...
    module: {
        loaders: [
            { test: /node_modules\/admin-config\/.*\.js$/, loader: 'babel' }
        ]
    }
};
```

## Running Tests

```sh
make test
```
