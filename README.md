# react-mind

[![TravisCI Build Status](https://travis-ci.org/mzabriskie/react-mind.svg?branch=master)](https://travis-ci.org/mzabriskie/react-mind)
[![Appveyor Build Status](https://ci.appveyor.com/api/projects/status/32r7s2skrgm9ubva?svg=true)](https://ci.appveyor.com/project/mzabriskie/react-mind)
[![npm downloads](https://img.shields.io/npm/dt/react-mind.svg?maxAge=2592000)](http://npmjs.com/package/react-mind)
[![gzip size](http://img.badgesize.io/https://npmcdn.com/react-mind/dist/react-mind.min.js?compression=gzip)]()

react-mind is a JavaScript library for building mind in react.

* **what:** react-mind only for building mind for react user

## start

`npm install react-mind`

## Examples

We have several examples [on the website](https://guimeisang.github.io/example/demo1.html). Here is the first one to get you started:

```js
import { Minder } from 'react-mind';

var mind = {
    "meta":{
        "name":"demo",
        "author":"792300489@qq.com",
        "version":"0.2",
    },
    "format":"node_tree",
    "data":{"id":"root","topic":"mind","children":[
            {"id":"easy","topic":"Easy","direction":"left","expanded":false,"children":[
                {"id":"easy1","topic":"Easy to show"},
                {"id":"easy2","topic":"Easy to edit"},
                {"id":"easy3","topic":"Easy to store"},
                {"id":"easy4","topic":"Easy to embed","children":[
                    {"id":"easy41","topic":"Easy to show"},
                    {"id":"easy42","topic":"Easy to edit"},
                    {"id":"easy43","topic":"Easy to store"},
                    {"id":"open44","topic":"BSD License","children":[
                        {"id":"open441","topic":"on GitHub"},
                        {"id":"open442","topic":"BSD License"}
                    ]},
                    {"id":"easy45","topic":"Easy to embed"}
                ]}
            ]},
            {"id":"open","topic":"Open Source","direction":"right","children":[
                {"id":"open1","topic":"on GitHub"},
                {"id":"open2","topic":"BSD License","children":[
                    {"id":"open21","topic":"on GitHub"},
                    {"id":"open22","topic":"BSD License","children":[
                        {"id":"open221","topic":"on GitHub"},
                        {"id":"open222","topic":"BSD License"}
                    ]}
                ]}
            ]},
            {"id":"powerful","topic":"Powerful","direction":"right","expanded":false,"children":[
                {"id":"powerful1","topic":"Base on Javascript"},
                {"id":"powerful2","topic":"Base on HTML5"},
                {"id":"powerful3","topic":"Depends on you","expanded":false,"children":[
                    {"id":"powerful31","topic":"Base on Javascript"},
                    {"id":"powerful32","topic":"Base on HTML5"},
                    {"id":"powerful33","topic":"Depends on you"}
                ]}
            ]},
            {"id":"other","topic":"test node","direction":"left","children":[
                {"id":"other1","topic":"I'm from ajax"},
                {"id":"other2","topic":"I can do everything"}
            ]}
        ]}
};
var options = {
    container:'mind_container',
    editable:true,
    theme:'primary'
}
var mind = Mind.show(options,mind);
```

## data

* `format`
> `node_tree`代表是树形的结构  `node_array` 代表数组的结构；

* `expanded`:
> 判断是否展开

* `direction`:
> 判断该节点是在左侧还是右侧；

## options

* `editable`
> 是否可以编辑，true为可以，false为不可以；

* `theme`
> 皮肤

## API
- `mind.get_data()`
> 获取数据

- `mind.set_readonly()`
> 设置为只读

- `mind.add_node("sub2","sub23", "new node", {"background-color":"red"});`
> 增加节点

- `mind.set_node_color('sub21', 'green', '#ccc');`
> 设置节点颜色

## TODO

- [ ] 实现组织结构图，实现鱼骨图等多种效果，用字段`structure`控制；
- [ ] 添加在渲染前，渲染后，展开，收起等事件的回调函数；
- [ ] 完善内部的事件系统；


## Installation

React-mind is available as the `react-mind` package on [npm](https://www.npmjs.com/).

## Contributing
this rope base on https://github.com/hizzgdev/jsmind @hizzgdev

### License

React-mind is [BSD licensed](./LICENSE). We also provide an additional [patent grant](./PATENTS).

React-mind documentation is [Creative Commons licensed](./LICENSE-docs).

Examples provided in this repository and in the documentation are [separately licensed](./LICENSE-examples).
