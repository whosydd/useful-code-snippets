# Useful code snippets

该插件主要记录一些我平时常用的代码片段，后续会进行补充

## 适用于 `js` `jsx` `ts` `tsx`

```js
req -> const moduleName = require('module')

mex -> module.exports = {}

ifs -> import fs from 'fs'

rfs -> const fs = require('fs')

ipath -> import path from 'path'

rpath -> const path = require('path')

ilodash -> import _ from 'lodash'

rlodash -> const _ = require('lodash')

af -> ()=>

eslint-disable -> /* eslint-disable */

eslint-disable-line -> /* eslint-disable-line */

eslint-disable-next-line -> /* eslint-disable-next-line */
```

## 仅适用于`js`

```js
strict -> 'use strict'

iife -> (function(){})()

did -> document.getElementById('id')

dcl -> document.getElementsByClassName('class')

dtag -> document.getElementsByTagName('tag')

dq -> document.querySelector()

dqa -> document.querySelectorAll()

dce -> document.createElement()

.al -> .addEventListener('load', function () {})
```

`express`

```js
const express = require("express");
const app = express();
const port = process.env.PORT || 5000;

app.get("/", (req, res) => res.send("Hey there!"));

app.listen(port, () => {
  console.log(`Server has started on port ${port}!!!`);
});
```
