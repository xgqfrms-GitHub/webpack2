# Output

https://webpack.js.org/concepts/#output


```js
const path = require('path');

module.exports = {
  entry: './path/to/my/entry/file.js',
  output: {
    path: path.resolve(__dirname, 'dist'),
    filename: 'my-first-webpack.bundle.js'
  }
};

```





https://webpack.js.org/concepts/output/

https://webpack.js.org/concepts/output/#output-path

```js

const config = {
  output: {
    filename: 'bundle.js',
    path: '/home/proj/public/assets'
  }
};

module.exports = config;

```












