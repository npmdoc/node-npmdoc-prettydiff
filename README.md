# api documentation for  [prettydiff (v99.0.1)](http://prettydiff.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-prettydiff.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-prettydiff) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-prettydiff.svg)](https://travis-ci.org/npmdoc/node-npmdoc-prettydiff)
#### Language aware code comparison tool for several web based languages. It also beautifies, minifies, and a few other things.

[![NPM](https://nodei.co/npm/prettydiff.png?downloads=true)](https://www.npmjs.com/package/prettydiff)

[![apidoc](https://npmdoc.github.io/node-npmdoc-prettydiff/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-prettydiff_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-prettydiff/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-prettydiff/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-prettydiff/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Austin Cheney",
        "email": "info@prettydiff.com",
        "url": "http://prettydiff.com/"
    },
    "bin": {
        "prettydiff": "./bin/prettydiff"
    },
    "bugs": {
        "url": "https://github.com/prettydiff/prettydiff/issues",
        "email": "info@prettydiff.com"
    },
    "config5082": {
        "beautify": true,
        "files": [
            ".bower.json",
            "bower.json",
            "prettydiff.js"
        ],
        "options": {
            "inchar": " ",
            "insize": 4,
            "vertical": true
        }
    },
    "dependencies": {},
    "description": "Language aware code comparison tool for several web based languages. It also beautifies, minifies, and a few other things.",
    "devDependencies": {
        "5082": "^1.0.0",
        "jslint": "^0.9.0"
    },
    "directories": {},
    "dist": {
        "shasum": "95a5d973358daea342161661401a79b87832b412",
        "tarball": "https://registry.npmjs.org/prettydiff/-/prettydiff-99.0.1.tgz"
    },
    "gitHead": "857775a6d2202e3ba080502f04fca1423914306e",
    "homepage": "http://prettydiff.com/",
    "keywords": [
        "beautify",
        "css",
        "diff",
        "es6",
        "html",
        "javascript",
        "jsx",
        "minify",
        "pretty diff",
        "pretty print",
        "pretty-print",
        "prettydiff",
        "xml"
    ],
    "license": "SEE LICENSE IN license.txt",
    "main": "prettydiff.js",
    "maintainers": [
        {
            "name": "austincheney",
            "email": "austin.cheney@us.army.mil"
        }
    ],
    "name": "prettydiff",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/prettydiff/prettydiff.git"
    },
    "scripts": {
        "test": "node test/lint.js"
    },
    "version": "99.0.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module prettydiff](#apidoc.module.prettydiff)
1.  [function <span class="apidocSignatureSpan">prettydiff.</span>api (x)](#apidoc.element.prettydiff.api)
1.  object <span class="apidocSignatureSpan">prettydiff.</span>csspretty
1.  object <span class="apidocSignatureSpan">prettydiff.</span>csvpretty
1.  object <span class="apidocSignatureSpan">prettydiff.</span>diffview
1.  object <span class="apidocSignatureSpan">prettydiff.</span>edition
1.  object <span class="apidocSignatureSpan">prettydiff.</span>jspretty
1.  object <span class="apidocSignatureSpan">prettydiff.</span>markuppretty
1.  object <span class="apidocSignatureSpan">prettydiff.</span>safeSort
1.  string <span class="apidocSignatureSpan">prettydiff.</span>report

#### [module prettydiff.csspretty](#apidoc.module.prettydiff.csspretty)
1.  [function <span class="apidocSignatureSpan">prettydiff.csspretty.</span>api (x)](#apidoc.element.prettydiff.csspretty.api)

#### [module prettydiff.csvpretty](#apidoc.module.prettydiff.csvpretty)
1.  [function <span class="apidocSignatureSpan">prettydiff.csvpretty.</span>api (x)](#apidoc.element.prettydiff.csvpretty.api)

#### [module prettydiff.diffview](#apidoc.module.prettydiff.diffview)
1.  [function <span class="apidocSignatureSpan">prettydiff.diffview.</span>api (x)](#apidoc.element.prettydiff.diffview.api)

#### [module prettydiff.jspretty](#apidoc.module.prettydiff.jspretty)
1.  boolean <span class="apidocSignatureSpan">prettydiff.jspretty.</span>jsxstatus
1.  [function <span class="apidocSignatureSpan">prettydiff.jspretty.</span>api (x)](#apidoc.element.prettydiff.jspretty.api)

#### [module prettydiff.markuppretty](#apidoc.module.prettydiff.markuppretty)
1.  [function <span class="apidocSignatureSpan">prettydiff.markuppretty.</span>api (x)](#apidoc.element.prettydiff.markuppretty.api)

#### [module prettydiff.safeSort](#apidoc.module.prettydiff.safeSort)
1.  [function <span class="apidocSignatureSpan">prettydiff.safeSort.</span>api (x)](#apidoc.element.prettydiff.safeSort.api)



# <a name="apidoc.module.prettydiff"></a>[module prettydiff](#apidoc.module.prettydiff)

#### <a name="apidoc.element.prettydiff.api"></a>[function <span class="apidocSignatureSpan">prettydiff.</span>api (x)](#apidoc.element.prettydiff.api)
- description and source-code
```javascript
function commonjs(x) {
    "use strict";
    return prettydiff(x);
}
```
- example usage
```shell
...

var prettydiff = require("prettydiff"),
    args       = {
        source: "asdf",
        diff  : "asdd",
        lang  : "text"
    },
    output     = prettydiff.api(args);

 Execute on command line with NodeJS:

npm install prettydiff -g     (global install)

prettydiff source:"c:\mydirectory\myfile.js" readmethod:"file" diff:"c:\myotherfile.js"
...
```



# <a name="apidoc.module.prettydiff.csspretty"></a>[module prettydiff.csspretty](#apidoc.module.prettydiff.csspretty)

#### <a name="apidoc.element.prettydiff.csspretty.api"></a>[function <span class="apidocSignatureSpan">prettydiff.csspretty.</span>api (x)](#apidoc.element.prettydiff.csspretty.api)
- description and source-code
```javascript
function commonjs(x) {
    "use strict";
    return csspretty(x);
}
```
- example usage
```shell
...

var prettydiff = require("prettydiff"),
    args       = {
        source: "asdf",
        diff  : "asdd",
        lang  : "text"
    },
    output     = prettydiff.api(args);

 Execute on command line with NodeJS:

npm install prettydiff -g     (global install)

prettydiff source:"c:\mydirectory\myfile.js" readmethod:"file" diff:"c:\myotherfile.js"
...
```



# <a name="apidoc.module.prettydiff.csvpretty"></a>[module prettydiff.csvpretty](#apidoc.module.prettydiff.csvpretty)

#### <a name="apidoc.element.prettydiff.csvpretty.api"></a>[function <span class="apidocSignatureSpan">prettydiff.csvpretty.</span>api (x)](#apidoc.element.prettydiff.csvpretty.api)
- description and source-code
```javascript
function commonjs(x) {
    "use strict";
    return csvpretty(x);
}
```
- example usage
```shell
...

var prettydiff = require("prettydiff"),
    args       = {
        source: "asdf",
        diff  : "asdd",
        lang  : "text"
    },
    output     = prettydiff.api(args);

 Execute on command line with NodeJS:

npm install prettydiff -g     (global install)

prettydiff source:"c:\mydirectory\myfile.js" readmethod:"file" diff:"c:\myotherfile.js"
...
```



# <a name="apidoc.module.prettydiff.diffview"></a>[module prettydiff.diffview](#apidoc.module.prettydiff.diffview)

#### <a name="apidoc.element.prettydiff.diffview.api"></a>[function <span class="apidocSignatureSpan">prettydiff.diffview.</span>api (x)](#apidoc.element.prettydiff.diffview.api)
- description and source-code
```javascript
function commonjs(x) {
    "use strict";
    return diffview(x);
}
```
- example usage
```shell
...

var prettydiff = require("prettydiff"),
    args       = {
        source: "asdf",
        diff  : "asdd",
        lang  : "text"
    },
    output     = prettydiff.api(args);

 Execute on command line with NodeJS:

npm install prettydiff -g     (global install)

prettydiff source:"c:\mydirectory\myfile.js" readmethod:"file" diff:"c:\myotherfile.js"
...
```



# <a name="apidoc.module.prettydiff.jspretty"></a>[module prettydiff.jspretty](#apidoc.module.prettydiff.jspretty)

#### <a name="apidoc.element.prettydiff.jspretty.api"></a>[function <span class="apidocSignatureSpan">prettydiff.jspretty.</span>api (x)](#apidoc.element.prettydiff.jspretty.api)
- description and source-code
```javascript
function commonjs(x) {
    "use strict";
    return jspretty(x);
}
```
- example usage
```shell
...

var prettydiff = require("prettydiff"),
    args       = {
        source: "asdf",
        diff  : "asdd",
        lang  : "text"
    },
    output     = prettydiff.api(args);

 Execute on command line with NodeJS:

npm install prettydiff -g     (global install)

prettydiff source:"c:\mydirectory\myfile.js" readmethod:"file" diff:"c:\myotherfile.js"
...
```



# <a name="apidoc.module.prettydiff.markuppretty"></a>[module prettydiff.markuppretty](#apidoc.module.prettydiff.markuppretty)

#### <a name="apidoc.element.prettydiff.markuppretty.api"></a>[function <span class="apidocSignatureSpan">prettydiff.markuppretty.</span>api (x)](#apidoc.element.prettydiff.markuppretty.api)
- description and source-code
```javascript
function commonjs(x) {
    "use strict";
    return markuppretty(x);
}
```
- example usage
```shell
...

var prettydiff = require("prettydiff"),
    args       = {
        source: "asdf",
        diff  : "asdd",
        lang  : "text"
    },
    output     = prettydiff.api(args);

 Execute on command line with NodeJS:

npm install prettydiff -g     (global install)

prettydiff source:"c:\mydirectory\myfile.js" readmethod:"file" diff:"c:\myotherfile.js"
...
```



# <a name="apidoc.module.prettydiff.safeSort"></a>[module prettydiff.safeSort](#apidoc.module.prettydiff.safeSort)

#### <a name="apidoc.element.prettydiff.safeSort.api"></a>[function <span class="apidocSignatureSpan">prettydiff.safeSort.</span>api (x)](#apidoc.element.prettydiff.safeSort.api)
- description and source-code
```javascript
function commonjs(x) {
    "use strict";
    return safeSort(x);
}
```
- example usage
```shell
...

var prettydiff = require("prettydiff"),
    args       = {
        source: "asdf",
        diff  : "asdd",
        lang  : "text"
    },
    output     = prettydiff.api(args);

 Execute on command line with NodeJS:

npm install prettydiff -g     (global install)

prettydiff source:"c:\mydirectory\myfile.js" readmethod:"file" diff:"c:\myotherfile.js"
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
