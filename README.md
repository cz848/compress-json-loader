
# Compress JSON loader

为小程序这种不需要以模块加载但是有压缩需求的 JSON 文件准备一份特殊的 JSON loader。

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
