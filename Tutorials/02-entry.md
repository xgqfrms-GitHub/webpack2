# Entry Points


https://webpack.js.org/concepts/entry-points/

```js

const config = {
  entry: './path/to/my/entry/file.js'
};

module.exports = config;


```


```js

const config = {
  entry: {
    main: './path/to/my/entry/file.js'
  }
};


```


```js

const config = {
  entry: {
    app: './src/app.js',
    vendors: './src/vendors.js'
  }
};

```


```js

const config = {
  entry: {
    pageOne: './src/pageOne/index.js',
    pageTwo: './src/pageTwo/index.js',
    pageThree: './src/pageThree/index.js'
  }
};

```


