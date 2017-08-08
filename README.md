# react-mind

[![TravisCI Build Status](https://travis-ci.org/mzabriskie/react-draggable.svg?branch=master)](https://travis-ci.org/mzabriskie/react-draggable)
[![Appveyor Build Status](https://ci.appveyor.com/api/projects/status/32r7s2skrgm9ubva?svg=true)](https://ci.appveyor.com/project/mzabriskie/react-draggable)
[![npm downloads](https://img.shields.io/npm/dt/react-draggable.svg?maxAge=2592000)](http://npmjs.com/package/react-draggable)
[![gzip size](http://img.badgesize.io/https://npmcdn.com/react-draggable/dist/react-draggable.min.js?compression=gzip)]()

react-mind is a JavaScript library for building mind in react.

* **what:** react-mind only for building mind for react user
* **other:** the react-mind not finished


## Examples

We have several examples [on the website](https://guimeisang.github.io/example/demo1.html). Here is the first one to get you started:

```js
import {Mind} from 'react-mind';

var mind = {
    "meta":{
        "name":"demo",
        "author":"hizzgdev@163.com",
        "version":"0.2",
    },
    "format":"node_array",
    "data":[
        {"id":"root", "isroot":true, "topic":"mind"},

        {"id":"sub1", "parentid":"root", "topic":"sub1", "background-color":"#0000ff"},
        {"id":"sub11", "parentid":"sub1", "topic":"sub11"},
        {"id":"sub12", "parentid":"sub1", "topic":"sub12"},
        {"id":"sub13", "parentid":"sub1", "topic":"sub13"},

        {"id":"sub2", "parentid":"root", "topic":"sub2"},
        {"id":"sub21", "parentid":"sub2", "topic":"sub21"},
        {"id":"sub22", "parentid":"sub2", "topic":"sub22","foreground-color":"#33ff33"},

        {"id":"sub3", "parentid":"root", "topic":"sub3"},
    ]
};
var options = {
    container:'mind_container',
    editable:true,
    theme:'primary'
}
var mind = Mind.show(options,mind);
```

## Installation

React-mind is available as the `react-mind` package on [npm](https://www.npmjs.com/).

## Contributing
https://github.com/hizzgdev/jsmind @hizzgdev


### License

React-mind is [BSD licensed](./LICENSE). We also provide an additional [patent grant](./PATENTS).

React-mind documentation is [Creative Commons licensed](./LICENSE-docs).

Examples provided in this repository and in the documentation are [separately licensed](./LICENSE-examples).
