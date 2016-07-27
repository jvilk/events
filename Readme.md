# events [![Build Status](https://travis-ci.org/Gozala/events.png?branch=master)](https://travis-ci.org/Gozala/events)

Node's event emitter for all engines. Modified to include an ES6 version.

## Breaking Changes ##

ES6 modules do not let you export an object as the module. Thus,
the following will not work if you are using the non-ES6 version:

```javascript
var EventEmitter = require('events');
var emitter = new EventEmitter();
```

Instead, do the following:

```javascript
var EventEmitter = require('events').EventEmitter;
var emitter = new EventEmitter();
```

## Install ##

```
npm install events
```

## Require ##

```javascript
var EventEmitter = require('events').EventEmitter
```

## Usage ##

See the [node.js event emitter docs](http://nodejs.org/api/events.html)
