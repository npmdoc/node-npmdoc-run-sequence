# api documentation for  [run-sequence (v1.2.2)](https://github.com/OverZealous/run-sequence)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-run-sequence.svg)](https://travis-ci.org/npmdoc/node-npmdoc-run-sequence)
#### Run a series of dependent gulp tasks in order

[![NPM](https://nodei.co/npm/run-sequence.png?downloads=true)](https://www.npmjs.com/package/run-sequence)

[![apidoc](https://npmdoc.github.io/node-npmdoc-run-sequence/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-run_sequence_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-run-sequence/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-run-sequence/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Phil DeJarnett",
        "url": "http://overzealous.com/"
    },
    "bugs": {
        "url": "https://github.com/OverZealous/run-sequence/issues"
    },
    "dependencies": {
        "chalk": "*",
        "gulp-util": "*"
    },
    "description": "Run a series of dependent gulp tasks in order",
    "devDependencies": {
        "gulp": "*",
        "mocha": "*",
        "should": "*"
    },
    "directories": {},
    "dist": {
        "shasum": "5095a0bebe98733b0140bd08dd80ec030ddacdeb",
        "tarball": "https://registry.npmjs.org/run-sequence/-/run-sequence-1.2.2.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "gitHead": "2238f6aea94c201173a99a4ccc1f2791c38531a1",
    "homepage": "https://github.com/OverZealous/run-sequence",
    "keywords": [
        "gulpfriendly",
        "pipe",
        "sequence",
        "gulp",
        "orchestrator"
    ],
    "license": "MIT",
    "main": "./index.js",
    "maintainers": [
        {
            "name": "overzealous",
            "email": "phil@overzealous.com"
        }
    ],
    "name": "run-sequence",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/OverZealous/run-sequence.git"
    },
    "scripts": {
        "test": "mocha --reporter spec"
    },
    "version": "1.2.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module run-sequence](#apidoc.module.run-sequence)
1.  [function <span class="apidocSignatureSpan">run-sequence.</span>use (gulp)](#apidoc.element.run-sequence.use)



# <a name="apidoc.module.run-sequence"></a>[module run-sequence](#apidoc.module.run-sequence)

#### <a name="apidoc.element.run-sequence.use"></a>[function <span class="apidocSignatureSpan">run-sequence.</span>use (gulp)](#apidoc.element.run-sequence.use)
- description and source-code
```javascript
use = function (gulp) {
	return runSequence.bind(null, gulp);
}
```
- example usage
```shell
...
If you have a complex gulp setup with your tasks split up across different files, you may get the error that 'run-sequence' is unable
 to find your tasks.  In this case, you can configure 'run-sequence' to look at the gulp within the submodule, like so:

'''js
// submodule tasks/mygulptask.js

var gulp = require('gulp'), // might be a different instance than the toplevel one
    // this uses the gulp you provide
    runSequence = require('run-sequence').use(gulp);

    // ...and then use normally
    runSequence('subtask1', 'subtask2');
'''

## LICENSE
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
