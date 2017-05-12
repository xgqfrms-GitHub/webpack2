# webpack 2 Tutorials (2017 version)


## `ExtractTextWebpackPlugin`


```js

// ExtractTextWebpackPlugin

https://github.com/xgqfrms-GitHub/webgeeker/tree/gh-pages/webpack2

https://doc.webpack-china.org/guides/migrating/

https://github.com/xgqfrms-GitHub/webgeeker/issues/5

https://www.youtube.com/watch?v=JdGnYNtuEtE

https://www.youtube.com/watch?v=eWmkBNBTbMM


https://doc.webpack-china.org/guides/migrating/#extracttextwebpackplugin-



const ExtractTextPlugin = require('extract-text-webpack-plugin');

module.exports = {
    module: {
        rules: [{
            test: /\.scss$/,
            use: ExtractTextPlugin.extract({
                use: ['style-loader', 'css-loader', 'sass-loader'],
                fallback: "style-loader",
                publicPath: "/dist"
            })
        }]
    },
    devtool: "source-map",
    plugins: [
        new ExtractTextPlugin({
            filename: "bundle.css",
            disable: false,
            allChunks: true
        }),
        new UglifyJsPlugin({
            sourceMap: true,
            compress: {
                warnings: true
            }
        }),
        new webpack.LoaderOptionsPlugin({
            minimize: true
        }),
        new webpack.BannerPlugin({
            banner: 'Banner', 
            raw: true, 
            entryOnly: true
        })
    ]
}






```










