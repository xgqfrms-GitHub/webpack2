# webpack 2 


https://webpack.js.org/guides/migrating/

https://github.com/webpack/webpack/issues/4475

https://survivejs.com/webpack/introduction/
https://survivejs.com/webpack/developing/getting-started/
https://survivejs.com/webpack/optimizing/adding-hashes-to-filenames/

https://survivejs.com/webpack/output/multiple-pages/

http://zhaoda.net/webpack-handbook/loader.html

https://doc.webpack-china.org/



```js

'use strict';
const webpack = require("webpack");
module.exports = {
    context: __dirname + "/src",
    entry: {
        app: "./app.js",
    },
    output: {
        path: __dirname + "/dist",
        filename: "[name].[chunkhash].bundle.js",
    },
    rules: [
        {
            test: /\.scss$/,
            use: [
                "style-loader",
                "css-loader",
                "sass-loader"
            ]
        },
        {
            test: /\.jxs$/,
            use: [
                "babel-loader"
            ],
            options: {
                modules: true
            }
        }
    ],
    devtool: "source-map",
    plugins: [
        new UglifyJsPlugin({
            sourceMap: true,
            warnings: true
        }),
        new webpack.LoaderOptionsPlugin({
            minimize: true
        })
    ]
};

```

## context 指定entry的root文件夹 src

## __dirname指的是项目的根目录


## path 指定 output 的root文件夹 dist

## [name] 是 占位符 自动替换为 entry 下的相同的文件名


## 通配符 * 




```sh
$ webpack -p
```

chunkFilename: '[name].[chunkhash:8].js',
filename: '[name].[chunkhash:8].js',
filename: '[name].[contenthash:8].css',





























s













































