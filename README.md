# npmdoc-purify-css

#### api documentation for  [purify-css (v1.1.9)](https://github.com/purifycss/purifycss)  [![npm package](https://img.shields.io/npm/v/npmdoc-purify-css.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-purify-css) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-purify-css.svg)](https://travis-ci.org/npmdoc/node-npmdoc-purify-css)

#### Removed unused css. Compatible with single-page apps.

[![NPM](https://nodei.co/npm/purify-css.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/purify-css)

- [https://npmdoc.github.io/node-npmdoc-purify-css/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-purify-css/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-purify-css/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-purify-css/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-purify-css/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-purify-css/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Kenny Tran, Matthew Rourke, Phoebe Li"
    },
    "bin": {
        "purifycss": "./bin/purifycss"
    },
    "bugs": {
        "url": "https://github.com/purifycss/purifycss/issues"
    },
    "dependencies": {
        "clean-css": "^3.2.10",
        "glob": "^6.0.4",
        "rework": "^1.0.1",
        "uglifyjs": "^2.4.10",
        "yargs": "^3.10.0"
    },
    "description": "Removed unused css. Compatible with single-page apps.",
    "devDependencies": {
        "chai": "^3.0.0",
        "eslint": "^0.24.1",
        "mocha": "^2.2.5"
    },
    "directories": {},
    "dist": {
        "shasum": "46c9acd8940f3076c0c346c027e286f996168357",
        "tarball": "https://registry.npmjs.org/purify-css/-/purify-css-1.1.9.tgz"
    },
    "files": [
        "bin",
        "src",
        "LICENSE",
        "package.json",
        "README.md"
    ],
    "gitHead": "212de957dbfbc20d15b8ed47c79f76600a83c803",
    "homepage": "https://github.com/purifycss/purifycss",
    "keywords": [
        "optimize",
        "css",
        "remove",
        "unused"
    ],
    "license": "MIT",
    "main": "./src/purifycss.js",
    "maintainers": [
        {
            "name": "kennyt"
        }
    ],
    "name": "purify-css",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/purifycss/purifycss.git"
    },
    "scripts": {
        "pretest": "eslint src && eslint bin/purifycss",
        "test": "node ./node_modules/mocha/bin/mocha"
    },
    "version": "1.1.9"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
