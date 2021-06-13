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

gid -> document.getElementById('id')

gcl -> document.getElementsByClassName('class')

gtag -> document.getElementsByTagName('tag')

qs -> document.querySelector()

qsa -> document.querySelectorAll()

ce -> document.createElement()

.al -> .addEventListener('load', function () {})

express ->
    const express = require('express')
	const app = express()
	const port = process.env.PORT || 5000

	app.get('/', (req, res) => res.send('Hey there!'))

	app.listen(port, () => { console.log(`Server has started on port ${port}!!!`) })
```

