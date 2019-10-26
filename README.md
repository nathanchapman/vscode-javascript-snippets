# JavaScript Snippets for VS Code

[![Version](https://img.shields.io/vscode-marketplace/v/nathanchapman.JavaScriptSnippets.svg)](https://marketplace.visualstudio.com/items?itemName=nathanchapman.JavaScriptSnippets)
[![Downloads](https://img.shields.io/vscode-marketplace/d/nathanchapman.JavaScriptSnippets.svg)](https://marketplace.visualstudio.com/items?itemName=nathanchapman.JavaScriptSnippets)
[![Rating](https://img.shields.io/vscode-marketplace/r/nathanchapman.JavaScriptSnippets.svg)](https://marketplace.visualstudio.com/items?itemName=nathanchapman.JavaScriptSnippets)

## Setup

Just install this package from the [Extension Marketplace](https://marketplace.visualstudio.com/VSCode), then make sure to add `"editor.snippetSuggestions": "top"` to your user settings to see these snippets on top in the suggestion popover.

## Snippets

Snippets are optimized to be short and easy to remember.

Below is a list of all available snippets and the triggers of each one. The **⇥** means the `TAB` key.

### Declarations
#### `v⇥` var statement
```javascript
var ${0}
```

#### `v=⇥` var assignment
```javascript
var ${1:name} = ${2:value};
```

#### `l⇥` let statement
```javascript
let ${0}
```

#### `l=⇥` let assignment
```javascript
let ${1:name} = ${2:value};
```

#### `dl=⇥` destructuring let assignment
```javascript
let {${1:name}} = ${2:value};
```

#### `co⇥` const statement
```javascript
const ${0}
```

#### `co=⇥` const assignment
```javascript
const ${1:name} = ${2:value};
```

#### `dco=⇥` destructuring const assignment
```javascript
const {${1:name}} = ${2:value};
```

### Flow Control
#### `if⇥` if statement
```javascript
if (${1:condition}) {
	${0}
}
```

#### `el⇥` else statement
```javascript
else {
	${0}
}
```

#### `ife⇥` if/else statement
```javascript
if (${1:condition}) {
	${0}
} else {
	
}
```

#### `ei⇥` else if statement
```javascript
else if (${1:condition}) {
	${0}
}
```

#### `ter⇥` ternary operator
```javascript
${1:condition} ? ${2:expression} : ${3:expression};
```

#### `fl⇥` for loop
```javascript
for (let ${1:i} = 0, ${2:len} = ${3:iterable}.length; ${1:i} < ${2:len}; ${1:i}++) {
	${0}
}
```

#### `rfl⇥` reverse for loop
```javascript
for (let ${1:i} = ${2:iterable}.length - 1; ${1:i} >= 0; ${1:i}--) {
	${0}
}
```

#### `fi⇥` for in loop
```javascript
for (let ${1:key} in ${2:array}) {
	if (${2:array}.hasOwnProperty(${1:key})) {
		${0}
	}
}
```

},
#### `fo⇥` for of loop (ES6)
```javascript
for (let ${1:key} of ${2:array}) {
	${0}
}
```

#### `wl⇥` while loop
```javascript
while (${1:condition}) {
	${0}
}
```

#### `tc⇥` try/catch
```javascript
try {
	${0}
} catch (${1:err}) {
	
}
```

#### `tf⇥` try/finally
```javascript
try {
	${0}
} finally {
	
}
```

#### `tcf⇥` try/catch/finally
```javascript
try {
	${0}
} catch (${1:err}) {
	
} finally {
	
}
```

#### `sw⇥` switch case
```javascript
switch (${1:expr}) {
	case ${2:value}:
		return $0;
	default:
		return;
}
```

### Functions
#### `f⇥` anonymous function
```javascript
function (${1:arguments}) {
	${0}
}
```

#### `fn⇥` named function
```javascript
function ${1:name}(${2:arguments}) {
	${0}
}
```

#### `iife⇥` immediately-invoked function expression (IIFE)
```javascript
((${1:arguments}) => {
	${0}
})(${2});
```

#### `fa⇥` function apply
```javascript
${1:fn}.apply(${2:this}, ${3:arguments})
```

#### `fc⇥` function call
```javascript
${1:fn}.call(${2:this}, ${3:arguments})
```

#### `fb⇥` function bind
```javascript
${1:fn}.bind(${2:this}, ${3:arguments})
```

#### `af⇥` arrow function (ES6)
```javascript
(${1:arguments}) => ${2:statement}
```

#### `afb⇥` arrow function with body (ES6)
```javascript
(${1:arguments}) => {
	${0}
}
```

#### `gf⇥` generator function (ES6)
```javascript
function* (${1:arguments}) {
	${0}
}
```

#### `gfn⇥` named generator function (ES6)
```javascript
function* ${1:name}(${2:arguments}) {
	${0}
}
```

### Iterables
#### `seq⇥` sequence of 0..n
```javascript
[...Array(${1:length}).keys()]${0}
```

#### `fe⇥` forEach loop
```javascript
${1}.forEach((${2:item}) => {
	${0}
});
```

#### `map⇥` map
```javascript
${1}.map((${2:item}) => {
	${0}
});
```

#### `reduce⇥` reduce
```javascript
${1}.reduce((${2:previous}, ${3:current}) => {
	${0}
}${4:, initial});
```

#### `filter⇥` filter
```javascript
${1}.filter(${2:item} => {
	${0}
});
```

#### `find⇥` find
```javascript
${1}.find(${2:item} => {
	${0}
});
```

### Objects and Classes
#### `ol⇥` object literal
```javascript
{
	kv${0}
};
```

#### `slol⇥` same-line object literal
```javascript
{ kv${0} };
```

#### `kv⇥` key/value pair
```javascript
${1:key}: ${2:value},
```

#### `c⇥` class (ES6)
```javascript
class ${1:name} {
	constructor(${2:arguments}) {
		${0}
	}
}
```

#### `cex⇥` child class (ES6)
```javascript
class ${1:name} extends ${2:base} {
	constructor(${3:arguments}) {
		super(${3:arguments});
		${0}
	}
}
```

#### `ctor⇥` class constructor (ES6)
```javascript
constructor(${1:arguments}) {
	super(${1:arguments});
	${0}
}
```

#### `m⇥` method (ES6 syntax)
```javascript
${1:method}(${2:arguments}) {
	${0}
}
```

#### `get⇥` getter (ES6 syntax)
```javascript
get ${1:property}() {
	${0}
}
```

#### `set⇥` setter (ES6 syntax)
```javascript
set ${1:property}(${2:value}) {
	${0}
}
```

#### `gs⇥` getter and setter (ES6 syntax)
```javascript
get ${1:property}() {
	${0}
}
set ${1:property}(${2:value}) {
	
}
```

#### `pctor⇥` prototypal constructor
```javascript
var ${1:Class} = function(${2:arguments}) {
	${0}
};
```

#### `proto⇥` prototype method
```javascript
${1:Class}.prototype.${2:method} = function(${3:arguments}) {
	${0}
};
```

#### `oa⇥` Object.assign
```javascript
Object.assign(${1:dest}, ${2:source})
```

#### `oc⇥` Object.assign copy (shallow clone)
```javascript
Object.assign({}, ${1:original}, ${2:source})
```

### Returning values
#### `r⇥` return
```javascript
return ${0};
```

#### `rp⇥` return Promise (ES6)
```javascript
return new Promise((resolve, reject) => {
	${0}
});
```

#### `rc⇥` return complex value (such as JSX components)
```javascript
return (
	${0}
);
```

### Types
#### `tof⇥` typeof
```javascript
typeof ${1:source} === '${2:undefined}'
```

#### `iof⇥` instanceof
```javascript
${1:source} instanceof ${2:Object}
```

### Promises
#### `pr⇥` Promise (ES6)
```javascript
new Promise((resolve, reject) => {
	${0}
})
```

#### `then⇥` Promise.then
```javascript
${1:promise}.then((${2:value}) => {
	${0}
})
```

#### `catch⇥` Promise.catch
```javascript
${1:promise}.catch((${2:err}) => {
	${0}
})
```

### ES6 Modules
#### `ex⇥` export (ES6)
```javascript
export ${1:member};
```

#### `exd⇥` export default (ES6)
```javascript
export default ${1:member};
```

#### `im⇥` import module (ES6)
```javascript
import ${1:*} from '${2:module}';
```

#### `ima⇥` import module as (ES6)
```javascript
import ${1:*} as ${2:name} from '${3:module}';
```

### Node.js
#### `cb⇥` Node.js style callback
```javascript
(err, ${1:value}) => {${0}}
```

#### `re⇥` require
```javascript
require('${1:module}');
```

#### `rel⇥` require local
```javascript
require('./${1:module}');
```

#### `req⇥` require assignment
```javascript
const ${1:module} = require('${1:module}');
```

#### `reql⇥` require assignment local
```javascript
const ${1:module} = require('./${1:module}');
```

#### `dreq⇥` destructuring require assignment
```javascript
const {${1:module}} = require('${1:module}');
```

#### `dreql⇥` destructuring require assignment local
```javascript
const {${1:module}} = require('./${1:module}');
```

#### `em⇥` exports.member
```javascript
exports.${1:member} = ${2:value};
```

#### `me⇥` module.exports
```javascript
module.exports = ${1:name};
```

#### `meo⇥` module exports object
```javascript
module.exports = {
	${1:member}
};
```

#### `on⇥` event handler
```javascript
${1:emitter}.on('${2:event}', (${3:arguments}) => {
	${0}
});
```

### BDD Testing (Mocha, Jasmine, etc.)
#### `desc⇥` describe
```javascript
describe('${1:description}', () => {
	${0}
});
```

#### `cont⇥` context
```javascript
context('${1:description}', () => {
	${0}
});
```

#### `it⇥` it
```javascript
it('${1:description}', () => {
	${0}
});
```

#### `its⇥` it synchronous
```javascript
it('${1:description}', () => {
	${0}
});
```

#### `ita⇥` it asynchronous
```javascript
it('${1:description}', (done) => {
	${0}
	done();
});
```

#### `bf⇥` before test suite
```javascript
before(() => {
	${0}
});
```

#### `bfe⇥` before each test
```javascript
beforeEach(() => {
	${0}
});
```

#### `aft⇥` after test suite
```javascript
after(() => {
	${0}
});
```

#### `afe⇥` after each test
```javascript
afterEach(() => {
	${0}
});
```

### Console
#### `cl⇥` console.log
```javascript
console.log(${0});
```

#### `ce⇥` console.error
```javascript
console.error(${0});
```

#### `cw⇥` console.warn
```javascript
console.warn(${0});
```

#### `cll⇥` console.log labeled
```javascript
console.log('${0}', ${0});
```

#### `cel⇥` console.error labeled
```javascript
console.error('${0}', ${0});
```

#### `cwl⇥` console.warn labeled
```javascript
console.warn('${0}', ${0});
```

### Timers
#### `st⇥` setTimeout
```javascript
setTimeout(() => {
	${0}
}, ${1:delay});
```

#### `si⇥` setInterval
```javascript
setInterval(() => {
	${0}
}, ${1:delay});
```

#### `sim⇥` setImmediate
```javascript
setImmediate(() => {
	${0}
});
```

#### `nt⇥` process nextTick
```javascript
process.nextTick(() => {
	${0}
});
```

### Miscellaneous
#### `us⇥` insert 'use strict' statement
```javascript
'use strict';
```

## Sponsorship 🎗

If you found this project useful, please consider becoming a [sponsor on GitHub](https://github.com/sponsors/nathanchapman).
