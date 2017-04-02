# api documentation for  [cli-color (v1.2.0)](https://github.com/medikoo/cli-color#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-cli-color.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cli-color) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cli-color.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cli-color)
#### Colors, formatting and other tools for the console

[![NPM](https://nodei.co/npm/cli-color.png?downloads=true)](https://www.npmjs.com/package/cli-color)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cli-color/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-cli-color_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cli-color/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-cli-color/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Mariusz Nowak",
        "email": "medyk@medikoo.com",
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
            "name": "medikoo",
            "email": "medikoo+npm@medikoo.com"
        }
    ],
    "name": "cli-color",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
1.  [function <span class="apidocSignatureSpan">cli-color.</span>sgr (code)](#apidoc.element.cli-color.sgr)

#### [module cli-color.sgr](#apidoc.module.cli-color.sgr)
1.  [function <span class="apidocSignatureSpan">cli-color.</span>sgr (code)](#apidoc.element.cli-color.sgr.sgr)
1.  [function <span class="apidocSignatureSpan">cli-color.sgr.</span>closeStyle (mods, code)](#apidoc.element.cli-color.sgr.closeStyle)
1.  [function <span class="apidocSignatureSpan">cli-color.sgr.</span>complete (mods, closerCodes)](#apidoc.element.cli-color.sgr.complete)
1.  [function <span class="apidocSignatureSpan">cli-color.sgr.</span>extractCode (csi)](#apidoc.element.cli-color.sgr.extractCode)
1.  [function <span class="apidocSignatureSpan">cli-color.sgr.</span>hasCSI (str)](#apidoc.element.cli-color.sgr.hasCSI)
1.  [function <span class="apidocSignatureSpan">cli-color.sgr.</span>openStyle (mods, code)](#apidoc.element.cli-color.sgr.openStyle)
1.  [function <span class="apidocSignatureSpan">cli-color.sgr.</span>prepend (mods)](#apidoc.element.cli-color.sgr.prepend)
1.  object <span class="apidocSignatureSpan">cli-color.sgr.</span>closers
1.  object <span class="apidocSignatureSpan">cli-color.sgr.</span>mods
1.  object <span class="apidocSignatureSpan">cli-color.sgr.</span>openers
1.  string <span class="apidocSignatureSpan">cli-color.sgr.</span>CSI



# <a name="apidoc.module.cli-color"></a>[module cli-color](#apidoc.module.cli-color)

#### <a name="apidoc.element.cli-color.sgr"></a>[function <span class="apidocSignatureSpan">cli-color.</span>sgr (code)](#apidoc.element.cli-color.sgr)
- description and source-code
```javascript
sgr = function (code) {
	return CSI + code + 'm';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cli-color.sgr"></a>[module cli-color.sgr](#apidoc.module.cli-color.sgr)

#### <a name="apidoc.element.cli-color.sgr.sgr"></a>[function <span class="apidocSignatureSpan">cli-color.</span>sgr (code)](#apidoc.element.cli-color.sgr.sgr)
- description and source-code
```javascript
sgr = function (code) {
	return CSI + code + 'm';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-color.sgr.closeStyle"></a>[function <span class="apidocSignatureSpan">cli-color.sgr.</span>closeStyle (mods, code)](#apidoc.element.cli-color.sgr.closeStyle)
- description and source-code
```javascript
closeStyle = function (mods, code) {
	forEachRight.call(mods, function (modPair, index) {
		if (modPair[1] === code) {
			mods.splice(index, 1);
		}
	});
}
```
- example usage
```shell
...
		return sgr(modPair[0]);
	});
};

/* complete non-closed openers with corresponding closers */
sgr.complete = function (mods, closerCodes) {
	closerCodes.forEach(function (code) {
		sgr.closeStyle(mods, code);
	});

	// mods must be closed from the last opened to first opened
	mods = mods.reverse();

	mods = mods.map(function (modPair, key) {
		return modPair[1];
...
```

#### <a name="apidoc.element.cli-color.sgr.complete"></a>[function <span class="apidocSignatureSpan">cli-color.sgr.</span>complete (mods, closerCodes)](#apidoc.element.cli-color.sgr.complete)
- description and source-code
```javascript
complete = function (mods, closerCodes) {
	closerCodes.forEach(function (code) {
		sgr.closeStyle(mods, code);
	});

	// mods must be closed from the last opened to first opened
	mods = mods.reverse();

	mods = mods.map(function (modPair, key) {
		return modPair[1];
	});

	// one closer can close many openers (31, 32 -> 39)
	mods = uniq.call(mods);

	return mods.map(sgr);
}
```
- example usage
```shell
...
		// closer CSIs for determining which pre/in-Openers must be closed
		inClosers:  []
	});

	sliced.seq = [].concat(
		sgr.prepend(sliced.preOpeners),
		sliced.seq,
		sgr.complete([].concat(sliced.preOpeners, sliced.inOpeners), sliced.inClosers)
	);

	return sliced.seq;
};

module.exports = function (str/*, begin, end*/) {
	var seq, begin = Number(arguments[1]), end = Number(arguments[2]), len;
...
```

#### <a name="apidoc.element.cli-color.sgr.extractCode"></a>[function <span class="apidocSignatureSpan">cli-color.sgr.</span>extractCode (csi)](#apidoc.element.cli-color.sgr.extractCode)
- description and source-code
```javascript
extractCode = function (csi) {
	var code = csi.slice(2, -1);
	code = Number(code);
	return code;
}
```
- example usage
```shell
...

				nextChunk = chunk.slice(relBegin, relEnd);
			}

			state.seq.push(nextChunk);
			state.index = index + chunk.length;
		} else {
			var code = sgr.extractCode(chunk.token);

			if (index <= begin) {
				if (code in sgr.openers) {
					sgr.openStyle(state.preOpeners, code);
				}
				if (code in sgr.closers) {
					sgr.closeStyle(state.preOpeners, code);
...
```

#### <a name="apidoc.element.cli-color.sgr.hasCSI"></a>[function <span class="apidocSignatureSpan">cli-color.sgr.</span>hasCSI (str)](#apidoc.element.cli-color.sgr.hasCSI)
- description and source-code
```javascript
hasCSI = function (str) {
	return includes.call(str, CSI);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli-color.sgr.openStyle"></a>[function <span class="apidocSignatureSpan">cli-color.sgr.</span>openStyle (mods, code)](#apidoc.element.cli-color.sgr.openStyle)
- description and source-code
```javascript
openStyle = function (mods, code) {
	mods.push(sgr.openers[code]);
}
```
- example usage
```shell
...
			state.seq.push(nextChunk);
			state.index = index + chunk.length;
		} else {
			var code = sgr.extractCode(chunk.token);

			if (index <= begin) {
				if (code in sgr.openers) {
					sgr.openStyle(state.preOpeners, code);
				}
				if (code in sgr.closers) {
					sgr.closeStyle(state.preOpeners, code);
				}
			} else if (index < end) {
				if (code in sgr.openers) {
					sgr.openStyle(state.inOpeners, code);
...
```

#### <a name="apidoc.element.cli-color.sgr.prepend"></a>[function <span class="apidocSignatureSpan">cli-color.sgr.</span>prepend (mods)](#apidoc.element.cli-color.sgr.prepend)
- description and source-code
```javascript
prepend = function (mods) {
	return mods.map(function (modPair, key) {
		return sgr(modPair[0]);
	});
}
```
- example usage
```shell
...

		// inClosers -> [ code ]
		// closer CSIs for determining which pre/in-Openers must be closed
		inClosers:  []
	});

	sliced.seq = [].concat(
		sgr.prepend(sliced.preOpeners),
		sliced.seq,
		sgr.complete([].concat(sliced.preOpeners, sliced.inOpeners), sliced.inClosers)
	);

	return sliced.seq;
};
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
