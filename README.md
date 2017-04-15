# api documentation for  [cli-color (v1.2.0)](https://github.com/medikoo/cli-color#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-cli-color.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cli-color) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cli-color.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cli-color)
#### Colors, formatting and other tools for the console

[![NPM](https://nodei.co/npm/cli-color.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/cli-color)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cli-color/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cli-color/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cli-color/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cli-color/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Mariusz Nowak",
        "url": "http://www.medikoo.com/"
    },
    "bugs": {
        "url": "https://github.com/medikoo/cli-color/issues"
    },
    "dependencies": {
        "ansi-regex": "^2.1.1",
        "d": "1",
        "es5-ext": "^0.10.12",
        "es6-iterator": "2",
        "memoizee": "^0.4.3",
        "timers-ext": "0.1"
    },
    "description": "Colors, formatting and other tools for the console",
    "devDependencies": {
        "tad": "^0.2.7",
        "xlint": "^0.2.2",
        "xlint-jslint-medikoo": "^0.1.4"
    },
    "directories": {},
    "dist": {
        "shasum": "3a5ae74fd76b6267af666e69e2afbbd01def34d1",
        "tarball": "https://registry.npmjs.org/cli-color/-/cli-color-1.2.0.tgz"
    },
    "gitHead": "7aae8aa90f59140d243fdd6d02253880d5281ad9",
    "homepage": "https://github.com/medikoo/cli-color#readme",
    "keywords": [
        "ansi",
        "color",
        "console",
        "terminal",
        "cli",
        "shell",
        "log",
        "logging",
        "xterm"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "medikoo"
        }
    ],
    "name": "cli-color",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/medikoo/cli-color.git"
    },
    "scripts": {
        "lint": "node node_modules/xlint/bin/xlint --linter=node_modules/xlint-jslint-medikoo/index.js --no-cache --no-stream",
        "lint-console": "node node_modules/xlint/bin/xlint --linter=node_modules/xlint-jslint-medikoo/index.js --watch",
        "test": "node ./node_modules/tad/bin/tad"
    },
    "version": "1.2.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module cli-color](#apidoc.module.cli-color)
1.  [function <span class="apidocSignatureSpan"></span>cli-color ()](#apidoc.element.cli-color.cli-color)
1.  [function <span class="apidocSignatureSpan">cli-color.</span>toString ()](#apidoc.element.cli-color.toString)



# <a name="apidoc.module.cli-color"></a>[module cli-color](#apidoc.module.cli-color)

#### <a name="apidoc.element.cli-color.cli-color"></a>[function <span class="apidocSignatureSpan"></span>cli-color ()](#apidoc.element.cli-color.cli-color)
- description and source-code
```javascript
function self() {
		var start = '', end = '', msg = join.call(arguments, ' '), conf = self._cliColorData
		  , hasAnsi = sgr.hasCSI(msg);
		forEach(conf, function (mod, key) {
			end    = sgr(mod[1]) + end;
			start += sgr(mod[0]);
			if (hasAnsi) {
				msg = msg.replace(getEndRe(mod[1]), variantModes[key] ? sgr(mod[0]) : '');
			}
		}, null, true);
		return start + msg + end;
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-color.toString"></a>[function <span class="apidocSignatureSpan">cli-color.</span>toString ()](#apidoc.element.cli-color.toString)
- description and source-code
```javascript
toString = function () {
    return toString;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
