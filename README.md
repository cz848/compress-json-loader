
# Compress JSON loader

为小程序这种不需要以模块加载但是有压缩需求的 JSON 文件准备一份特殊的 JSON loader。代码只是在 Webpack 的 (json-loader)[https://github.com/webpack-contrib/json-loader] 的基础上稍做修改

**webpack.config.js**
```js
module.exports = {
  module: {
    loaders: [
      {
        test: /\.json$/,
        loader: 'compress-json-loader'
      }
    ]
  }
}
```
