# react-mind

[![TravisCI Build Status](https://travis-ci.org/mzabriskie/react-draggable.svg?branch=master)](https://travis-ci.org/mzabriskie/react-draggable)
[![Appveyor Build Status](https://ci.appveyor.com/api/projects/status/32r7s2skrgm9ubva?svg=true)](https://ci.appveyor.com/project/mzabriskie/react-draggable)
[![npm downloads](https://img.shields.io/npm/dt/react-draggable.svg?maxAge=2592000)](http://npmjs.com/package/react-draggable)
[![gzip size](http://img.badgesize.io/https://npmcdn.com/react-draggable/dist/react-draggable.min.js?compression=gzip)]()

react-mind is a JavaScript library for building mind in react.

* **what:** react-mind only for building mind for react user
* **other:* the react-mind not finished


## Examples

We have several examples [on the website](https://facebook.github.io/react/). Here is the first one to get you started:

```js
class HelloMessage extends React.Component {
  render() {
    return <div>Hello {this.props.name}</div>;
  }
}

ReactDOM.render(
  <HelloMessage name="John" />,
  document.getElementById('container')
);
```

This example will render "Hello John" into a container on the page.

You'll notice that we used an HTML-like syntax; [we call it JSX](https://facebook.github.io/react/docs/introducing-jsx.html). JSX is not required to use React, but it makes code more readable, and writing it feels like writing HTML. We recommend using [Babel](https://babeljs.io/) with a [React preset](https://babeljs.io/docs/plugins/preset-react/) to convert JSX into native JavaScript for browsers to digest.

## Installation

React is available as the `react` package on [npm](https://www.npmjs.com/). It is also available on a [CDN](https://facebook.github.io/react/docs/installation.html#using-a-cdn).

React is flexible and can be used in a variety of projects. You can create new apps with it, but you can also gradually introduce it into an existing codebase without doing a rewrite.

The recommended way to install React depends on your project. Here you can find short guides for the most common scenarios:

* [Trying Out React](https://facebook.github.io/react/docs/installation.html#trying-out-react)
* [Creating a New Application](https://facebook.github.io/react/docs/installation.html#creating-a-new-application)
* [Adding React to an Existing Application](https://facebook.github.io/react/docs/installation.html#adding-react-to-an-existing-application)

## Contributing

The main purpose of this repository is to continue to evolve React core, making it faster and easier to use. Development of React happens in the open on GitHub, and we are grateful to the community for contributing bugfixes and improvements. Read below to learn how you can take part in improving React.

### [Code of Conduct](https://code.facebook.com/codeofconduct)

Facebook has adopted a Code of Conduct that we expect project participants to adhere to. Please read [the full text](https://code.facebook.com/codeofconduct) so that you can understand what actions will and will not be tolerated.

### Contributing Guide

Read our [contributing guide](https://facebook.github.io/react/contributing/how-to-contribute.html) to learn about our development process, how to propose bugfixes and improvements, and how to build and test your changes to React.

### Beginner Friendly Bugs

To help you get your feet wet and get you familiar with our contribution process, we have a list of [beginner friendly bugs](https://github.com/facebook/react/labels/Difficulty%3A%20beginner) that contain bugs which are fairly easy to fix. This is a great place to get started.

### License

React is [BSD licensed](./LICENSE). We also provide an additional [patent grant](./PATENTS).

React documentation is [Creative Commons licensed](./LICENSE-docs).

Examples provided in this repository and in the documentation are [separately licensed](./LICENSE-examples).
