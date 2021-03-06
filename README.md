# node-ranger


[![npm](https://img.shields.io/npm/v/node-ranger.svg?style=flat)](https://npmjs.org/package/node-ranger)
[![npm](https://img.shields.io/npm/dm/node-ranger.svg?style=flat)](https://npmjs.org/package/node-ranger)
[![Build Status](https://travis-ci.org/andela-abankole/node-ranger.svg?branch=master&style=flat)](https://travis-ci.org/andela-abankole/ranger)


*Range function for Node.js*


![Frankenstein Sketch](_static/frankenstein-sketch.png)


## Installation

To install `ranger` using [npm](https://www.npmjs.org/), simply run:

```console
$ npm install node-ranger
```

In the root of your project directory.


## Usage

Once you have `ranger` installed, you can use it to easily get an Array or Object of numbers providing three arguments, a start, end and step value. The function call ranger.getArray(1, 10, 2) should return [1, 3, 5, 7, 9]:

```javascript
var ranger = require('ranger');

console.log(ranger.getArray(1, 10, 2));
// [1, 3, 5, 7, 9]
```

Want the range as a Object? No Problem!

```javascript
var ranger = require('ranger');

console.log(ranger.getObject(1, 10, 2));
// {0: 1, 1: 3, 2: 5, 3: 7, 4: 9}
```

The methods above use the reduce method, if you prefer the native `for..loop`:

```javascript
var ranger = require('ranger');

console.log(ranger.fill(1, 10, 2));
// [1, 3, 5, 7, 9]
```


## Author's Journal
- I had a hard time finding the right name for each method.
- I didn't want to call this library `ranger`, but I don't have
  any ideas. ¯\\_(ツ)_/¯
- Implementing Async soon!


## Changelog
v1.0.0: 6/10/16, 11:55 AM

```text
  - Initial Release
```
