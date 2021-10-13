# Useful code snippets

该插件主要记录一些我平时常用的代码片段，后续会进行补充

## 适用于 `js` `jsx` `ts` `tsx` `html` `vue`

### exprot

```js
mex -> module.exports = {}

exd -> export default

exo -> export {}

enf -> export const funcName = (params) => {}

edf -> export default (params) => {}
```

### import

```js
req -> const moduleName = require('module')

imp -> import moduleName from 'module'

ifs -> import fs from 'fs'

rfs -> const fs = require('fs')

ipath -> import path from 'path'

rpath -> const path = require('path')

ilodash -> import _ from 'lodash'

rlodash -> const _ = require('lodash')

iaxios -> import axios from 'axios'

raxios -> const axios = require('axios')

dotenv -> require('dotenv').config()
```

### function

```js
af -> () =>

afn -> () => {}

cfn -> const funcName = () => {}

rfn -> return () => {}
```

### eslint

```js
eslint-disable -> /* eslint-disable */

eslint-disable-line -> /* eslint-disable-line */

eslint-disable-next-line -> /* eslint-disable-next-line */
```

### array

```js
.forEach -> .forEach((item) => )

.map -> .map((item) => )

.filter -> .filter((item) => )

.reduce -> .reduce((item) => , )

fof -> for (let itemName of objectName) {}

fin -> for (let itemName in objectName) {}
```

### promise

```js
rprom -> return new Promise((resolve, reject) => {})

.thenc -> .then((res) => ).catch((err) => )
```

### console

```js
cl -> console.log(' -->', )
```

### other

```js
sto -> setTimeout(() =>  , timeout)

sti -> setInterval(() =>  , interval)
```

### hf ( 将header字符串格式化为对象)

```js
const headers = {}
header.split('\n').map(item => {
  const h = item.split(': ')
  Object.assign(headers, { [h[0]]: h[1] })
})
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

## react 仅适用于 `jsx` `tsx`

> react 部分全部来自于[ES7 React/Redux/GraphQL/React-Native snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)
>
> 针对个人使用情况仅添加了目前我用的比较多的代码片段

```js
cp -> const {} = this.props

cs -> const {} = this.state

imr -> import React from 'react'

impt -> import PropTypes from 'prop-types'

est -> state = {}

cref -> this.refNameRef = React.createRef()

fref -> const ref = React.createRef()

sst -> this.setState({})

ssf -> this.setState((state,props) => {})
```

### rcc

```js
import React, { Component } from "react";

export default class test extends Component {
  render() {
    return <div></div>;
  }
}
```

### rccp

```js
import React, { Component } from "react";
import PropTypes from "prop-types";

export default class test extends Component {
  static propTypes = {
    prop: PropTypes,
  };

  render() {
    return <div></div>;
  }
}
```

### rce

```js
import React, { Component } from "react";

export class test extends Component {
  render() {
    return <div></div>;
  }
}

export default test;
```

### rcep

```js
import React, { Component } from "react";
import PropTypes from "prop-types";

export class test extends Component {
  static propTypes = {};

  render() {
    return <div></div>;
  }
}

export default test;
```

### rfc

```js
import React from "react";

export default function test() {
  return <div></div>;
}
```

### rfce

```js
import React from "react";

function test() {
  return <div></div>;
}

export default test;
```

### rfcp

```js
import React from "react";
import PropTypes from "prop-types";

function test(props) {
  return <div></div>;
}

test.propTypes = {};

export default test;
```

### rpc

```js
import React, { PureComponent } from "react";

export default class test extends PureComponent {
  render() {
    return <div></div>;
  }
}
```

### rpce

```js
import React, { PureComponent } from "react";

export class test extends PureComponent {
  render() {
    return <div></div>;
  }
}

export default test;
```

### rpcp

```js
import React, { PureComponent } from "react";
import PropTypes from "prop-types";

export default class test extends PureComponent {
  static propTypes = {};

  render() {
    return <div></div>;
  }
}
```

### reduxmap

```js
const mapStateToProps = (state) => ({});

const mapDispatchToProps = {};
```

## Thanks

[ES7 React/Redux/GraphQL/React-Native snippets](https://marketplace.visualstudio.com/items?itemName=dsznajder.es7-react-js-snippets)

Icons made by <a href="https://www.freepik.com" title="Freepik">Freepik</a> from <a href="https://www.flaticon.com/" title="Flaticon">www.flaticon.com</a>

