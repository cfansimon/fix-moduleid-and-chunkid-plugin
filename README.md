# fix-moduleid-and-chunkid-plugin

Make module id and chunk id fixed and changeless when add or remove modules.

## Usage

Install via npm:

```shell
npm install fix-moduleid-and-chunkid-plugin
```

And then require and provide to webpack:

```javascript
// in webpack.config.js or similar
var FixModuleIdAndChunkIdPlugin = require('fix-moduleid-and-chunkid-plugin');

module.exports = {
  //...
  plugins: [
    new FixModuleIdAndChunkIdPlugin()
  ]
  //...
};
```

After builded:

```javascipt
webpackJsonp(["course/manage/list"],[
/* 0 */
/***/ function(module, exports, __webpack_require__) {

    'use strict';

    __webpack_require__("9ba58fe4941a24a87be7");

    console.log('course manage list.jsx');

/***/ }
]);
```
