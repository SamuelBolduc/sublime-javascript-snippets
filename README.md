# NodeJS ES6 snippets for SublimeText

This is a fork of [JavaScript & NodeJS Snippets for Sublime Text 2/3](zenorocha/sublime-javascript-snippets) by Zeno Rocha, using the ES6 syntax and without the DOM snippets.

## Install

To install through [Package Control](http://wbond.net/sublime_packages/package_control),
search for **NodeJS ES6 snippets**. If you still don't have Package Control in Sublime Text, [go get it](http://wbond.net/sublime_packages/package_control/installation).

If you prefer to install it manually, you can download the package and put it inside your `Packages` directory. It should work but will not update automatically.

## Console

### [cd] console.dir

```javascript
console.dir(${1:obj});
```

### [ce] console.error

```javascript
console.error(${1:obj});
```

### [cl] console.log

```javascript
console.log(${1:obj});
```

### [cw] console.warn

```javascript
console.warn(${1:obj});
```

### [de] debugger

```javascript
debugger;
```

## Loop

### [fe] forEach

```javascript
${1:myArray}.forEach(${2:elem} => {
	${3}
});
```

### [fei] forEach with index

```javascript
${1:myArray}.forEach((${2:elem}, i) {
	${3}
});
```

### [fi] for in

```javascript
for (${1:prop} in ${2:obj}) {
	if (${2:obj}.hasOwnProperty(${1:prop})) {
		${3}
	}
}
```

## Function

### [fn] function

```javascript
function ${1:methodName}(${2:arguments}) {
	${3}
}
```

### [afn] anonymous function

```javascript
(${1:arguments}) => {
	${2}
}
```

### [pr] prototype

```javascript
${1:ClassName}.prototype.${2:methodName} = (${3:arguments}) => {
	${4}
}
```

### [call] function call

```javascript
${1:methodName}.call(${2:context}, ${3:arguments})
```

### [apply] function apply

```javascript
${1:methodName}.apply(${2:context}, [${3:arguments}])
```

### [ofn] function as a property of an object

```javascript
${1:functionName}(${2:arguments}) {
	${3}
}
```

## Timer

### [si] setInterval

```javascript
setInterval(() => {
	${2}
}, ${1:delay});
```

### [st] setTimeout

```javascript
setTimeout(() => {
	${2}
}, ${1:delay});
```

## NodeJS

### [ase] assert.equal

```javascript
assert.equal(${1:actual}, ${2:expected});
```

### [asd] assert.deepEqual

```javascript
assert.deepEqual(${1:actual}, ${2:expected});
```

### [asn] assert.notEqual

```javascript
assert.notEqual(${1:actual}, ${2:expected});
```

### [me] module.exports

```javascript
module.exports = ${1:name};
```

### [pe] process.exit

```javascript
process.exit(${1:code});
```

### [re] require

```javascript
require('${1:module}');
```
## BDD

### [desc] describe

```javascript
describe('${1:description}', () => {
	${2}
});
```
### [ita] it asynchronous

```javascript
it('${1:description}', done => {
	${2}
});
```

### [its] it synchronous

```javascript
it('${1:description}', () => {
	${2}
});
```

### [itp] it pending

```javascript
it('${1:description}');
```

## Misc

### [us] use strict

```javascript
'use strict';
```

## Contributing

1. Fork it!
2. Create your feature branch: `git checkout -b my-new-feature`
3. Commit your changes: `git commit -m 'Add some feature'`
4. Push to the branch: `git push origin my-new-feature`
5. Submit a pull request :D

## License

[MIT License](http://zenorocha.mit-license.org/) © Samuel Bolduc. Based on the work of [Zeno Rocha](https://github.com/zenorocha).
