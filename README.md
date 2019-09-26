# TypeError: Cannot read property '0' of undefined

The goal of this repo is to recreate a TypeError bug in Oboe.js 2.1.4 and later
which I found with the [Oboe.js](https://github.com/jimhigson/oboe.js) library.

Running this code will produce the following Error:

```bash
$ npm install
$ npm start

C:\..\obt\node_modules\oboe\dist\oboe-node.js:121
   return function(o) { return o[key]; };
                                ^

TypeError: Cannot read property '0' of undefined
    at C:\..\obt\node_modules\oboe\dist\oboe-node.js:121:33
    at appendBuiltContent (C:\..\obt\node_modules\oboe\dist\oboe-node.js:1455:15)
    at nodeOpened (C:\..\obt\node_modules\oboe\dist\oboe-node.js:1436:7)
    at C:\tmp\obt\node_modules\oboe\dist\oboe-node.js:1050:19
    at applyEach (C:\tmp\obt\node_modules\oboe\dist\oboe-node.js:496:20)
    at emit (C:\tmp\obt\node_modules\oboe\dist\oboe-node.js:1931:7)
    at emitError (C:\tmp\obt\node_modules\oboe\dist\oboe-node.js:630:9)
    at handleStreamEnd (C:\tmp\obt\node_modules\oboe\dist\oboe-node.js:665:7)
    at applyEach (C:\tmp\obt\node_modules\oboe\dist\oboe-node.js:496:20)
    at Object.emit (C:\tmp\obt\node_modules\oboe\dist\oboe-node.js:1931:7)
```

## Getting started

- Fork
- `$ npm install`
- `$ npm start`
