git-rev-sync
============

Synchronously get the current git commit hash, tag, or branch. Forked from [git-rev](https://github.com/tblobaum/git-rev).


## Example

```js
var git = require('git-rev-sync');

console.log(git.short());
// 75bf4ee

console.log(git.long());
// 75bf4eea9aa1a7fd6505d0d0aa43105feafa92ef

console.log(git.branch());
// master

console.log(git.tag());
// not implemented

console.log(git.log());
// not implemented
```

You can also run these examples via: `npm run examples`


## Install

`npm install git-rev-sync --save`


## Methods

``` js
var git = require('git-rev-sync');
```

#### short() &rarr; &lt;String&gt;

return the result of `git rev-parse --short HEAD`

#### long() &rarr; &lt;String&gt;

return the result of `git rev-parse HEAD`

#### branch() &rarr; &lt;String&gt;

return the current branch


## License

[MIT](https://github.com/kurttheviking/git-rev-sync/blob/master/LICENSE)
