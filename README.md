# api documentation for  [purify-css (v1.1.9)](https://github.com/purifycss/purifycss)  [![npm package](https://img.shields.io/npm/v/npmdoc-purify-css.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-purify-css) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-purify-css.svg)](https://travis-ci.org/npmdoc/node-npmdoc-purify-css)
#### Removed unused css. Compatible with single-page apps.

[![NPM](https://nodei.co/npm/purify-css.png?downloads=true)](https://www.npmjs.com/package/purify-css)

[![apidoc](https://npmdoc.github.io/node-npmdoc-purify-css/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-purify-css_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-purify-css/build/apidoc.html)

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
            "name": "kennyt",
            "email": "kenny8tran@gmail.com"
        }
    ],
    "name": "purify-css",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module purify-css](#apidoc.module.purify-css)
1.  [function <span class="apidocSignatureSpan">purify-css.</span>CssTreeWalker (code, plugins)](#apidoc.element.purify-css.CssTreeWalker)
1.  [function <span class="apidocSignatureSpan">purify-css.</span>SelectorFilter (contentWords, whitelist)](#apidoc.element.purify-css.SelectorFilter)
1.  object <span class="apidocSignatureSpan">purify-css.</span>CssTreeWalker.prototype
1.  object <span class="apidocSignatureSpan">purify-css.</span>SelectorFilter.prototype

#### [module purify-css.CssTreeWalker](#apidoc.module.purify-css.CssTreeWalker)
1.  [function <span class="apidocSignatureSpan">purify-css.</span>CssTreeWalker (code, plugins)](#apidoc.element.purify-css.CssTreeWalker.CssTreeWalker)

#### [module purify-css.CssTreeWalker.prototype](#apidoc.module.purify-css.CssTreeWalker.prototype)
1.  [function <span class="apidocSignatureSpan">purify-css.CssTreeWalker.prototype.</span>beginReading ()](#apidoc.element.purify-css.CssTreeWalker.prototype.beginReading)
1.  [function <span class="apidocSignatureSpan">purify-css.CssTreeWalker.prototype.</span>constructor (code, plugins)](#apidoc.element.purify-css.CssTreeWalker.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">purify-css.CssTreeWalker.prototype.</span>readPlugin (tree)](#apidoc.element.purify-css.CssTreeWalker.prototype.readPlugin)
1.  [function <span class="apidocSignatureSpan">purify-css.CssTreeWalker.prototype.</span>readRules (rules)](#apidoc.element.purify-css.CssTreeWalker.prototype.readRules)
1.  [function <span class="apidocSignatureSpan">purify-css.CssTreeWalker.prototype.</span>removeEmptyRules (rules)](#apidoc.element.purify-css.CssTreeWalker.prototype.removeEmptyRules)
1.  [function <span class="apidocSignatureSpan">purify-css.CssTreeWalker.prototype.</span>toString ()](#apidoc.element.purify-css.CssTreeWalker.prototype.toString)

#### [module purify-css.SelectorFilter](#apidoc.module.purify-css.SelectorFilter)
1.  [function <span class="apidocSignatureSpan">purify-css.</span>SelectorFilter (contentWords, whitelist)](#apidoc.element.purify-css.SelectorFilter.SelectorFilter)

#### [module purify-css.SelectorFilter.prototype](#apidoc.module.purify-css.SelectorFilter.prototype)
1.  [function <span class="apidocSignatureSpan">purify-css.SelectorFilter.prototype.</span>filterSelectors (selectors)](#apidoc.element.purify-css.SelectorFilter.prototype.filterSelectors)
1.  [function <span class="apidocSignatureSpan">purify-css.SelectorFilter.prototype.</span>initialize (CssSyntaxTree)](#apidoc.element.purify-css.SelectorFilter.prototype.initialize)
1.  [function <span class="apidocSignatureSpan">purify-css.SelectorFilter.prototype.</span>parseRule (selectors, rule)](#apidoc.element.purify-css.SelectorFilter.prototype.parseRule)
1.  [function <span class="apidocSignatureSpan">purify-css.SelectorFilter.prototype.</span>parseWhitelist (whitelist)](#apidoc.element.purify-css.SelectorFilter.prototype.parseWhitelist)



# <a name="apidoc.module.purify-css"></a>[module purify-css](#apidoc.module.purify-css)

#### <a name="apidoc.element.purify-css.CssTreeWalker"></a>[function <span class="apidocSignatureSpan">purify-css.</span>CssTreeWalker (code, plugins)](#apidoc.element.purify-css.CssTreeWalker)
- description and source-code
```javascript
CssTreeWalker = function (code, plugins) {
  EventEmitter.call(this);
  this.startingSource = code;
  this.ast = null;

  plugins.forEach(function (plugin) {
    plugin.initialize(this);
  }.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.purify-css.SelectorFilter"></a>[function <span class="apidocSignatureSpan">purify-css.</span>SelectorFilter (contentWords, whitelist)](#apidoc.element.purify-css.SelectorFilter)
- description and source-code
```javascript
SelectorFilter = function (contentWords, whitelist) {
  this.contentWords = contentWords;
  this.rejectedSelectors = [];
  this.wildcardWhitelist = [];

  this.parseWhitelist(whitelist);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.purify-css.CssTreeWalker"></a>[module purify-css.CssTreeWalker](#apidoc.module.purify-css.CssTreeWalker)

#### <a name="apidoc.element.purify-css.CssTreeWalker.CssTreeWalker"></a>[function <span class="apidocSignatureSpan">purify-css.</span>CssTreeWalker (code, plugins)](#apidoc.element.purify-css.CssTreeWalker.CssTreeWalker)
- description and source-code
```javascript
CssTreeWalker = function (code, plugins) {
  EventEmitter.call(this);
  this.startingSource = code;
  this.ast = null;

  plugins.forEach(function (plugin) {
    plugin.initialize(this);
  }.bind(this));
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.purify-css.CssTreeWalker.prototype"></a>[module purify-css.CssTreeWalker.prototype](#apidoc.module.purify-css.CssTreeWalker.prototype)

#### <a name="apidoc.element.purify-css.CssTreeWalker.prototype.beginReading"></a>[function <span class="apidocSignatureSpan">purify-css.CssTreeWalker.prototype.</span>beginReading ()](#apidoc.element.purify-css.CssTreeWalker.prototype.beginReading)
- description and source-code
```javascript
beginReading = function () {
  this.ast = rework(this.startingSource)
    .use(this.readPlugin.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.purify-css.CssTreeWalker.prototype.constructor"></a>[function <span class="apidocSignatureSpan">purify-css.CssTreeWalker.prototype.</span>constructor (code, plugins)](#apidoc.element.purify-css.CssTreeWalker.prototype.constructor)
- description and source-code
```javascript
constructor = function (code, plugins) {
  EventEmitter.call(this);
  this.startingSource = code;
  this.ast = null;

  plugins.forEach(function (plugin) {
    plugin.initialize(this);
  }.bind(this));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.purify-css.CssTreeWalker.prototype.readPlugin"></a>[function <span class="apidocSignatureSpan">purify-css.CssTreeWalker.prototype.</span>readPlugin (tree)](#apidoc.element.purify-css.CssTreeWalker.prototype.readPlugin)
- description and source-code
```javascript
readPlugin = function (tree) {
  this.readRules(tree.rules);
  this.removeEmptyRules(tree.rules);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.purify-css.CssTreeWalker.prototype.readRules"></a>[function <span class="apidocSignatureSpan">purify-css.CssTreeWalker.prototype.</span>readRules (rules)](#apidoc.element.purify-css.CssTreeWalker.prototype.readRules)
- description and source-code
```javascript
readRules = function (rules) {
  rules.forEach(function (rule) {
    var ruleType = rule.type;

    if (ruleType === RULE_TYPE) {
      this.emit('readRule', rule.selectors, rule);
    }

    if (ruleType === MEDIA_TYPE) {
      this.readRules(rule.rules);
    }
  }.bind(this));
}
```
- example usage
```shell
...

CssTreeWalker.prototype.beginReading = function () {
this.ast = rework(this.startingSource)
  .use(this.readPlugin.bind(this));
};

CssTreeWalker.prototype.readPlugin = function (tree) {
this.readRules(tree.rules);
this.removeEmptyRules(tree.rules);
};

CssTreeWalker.prototype.readRules = function (rules) {
rules.forEach(function (rule) {
  var ruleType = rule.type;
...
```

#### <a name="apidoc.element.purify-css.CssTreeWalker.prototype.removeEmptyRules"></a>[function <span class="apidocSignatureSpan">purify-css.CssTreeWalker.prototype.</span>removeEmptyRules (rules)](#apidoc.element.purify-css.CssTreeWalker.prototype.removeEmptyRules)
- description and source-code
```javascript
removeEmptyRules = function (rules) {
  var emptyRules = [];

  rules.forEach(function (rule) {
    var ruleType = rule.type;

    if (ruleType === RULE_TYPE && rule.selectors.length === 0) {
      emptyRules.push(rule);
    }

    if (ruleType === MEDIA_TYPE) {
      this.removeEmptyRules(rule.rules);
      if (rule.rules.length === 0) {
        emptyRules.push(rule);
      }
    }
  }.bind(this));

  emptyRules.forEach(function (emptyRule) {
    var index = rules.indexOf(emptyRule);
    rules.splice(index, 1);
  });
}
```
- example usage
```shell
...
CssTreeWalker.prototype.beginReading = function () {
  this.ast = rework(this.startingSource)
.use(this.readPlugin.bind(this));
};

CssTreeWalker.prototype.readPlugin = function (tree) {
  this.readRules(tree.rules);
  this.removeEmptyRules(tree.rules);
};

CssTreeWalker.prototype.readRules = function (rules) {
  rules.forEach(function (rule) {
var ruleType = rule.type;

if (ruleType === RULE_TYPE) {
...
```

#### <a name="apidoc.element.purify-css.CssTreeWalker.prototype.toString"></a>[function <span class="apidocSignatureSpan">purify-css.CssTreeWalker.prototype.</span>toString ()](#apidoc.element.purify-css.CssTreeWalker.prototype.toString)
- description and source-code
```javascript
toString = function () {
  if (this.ast) {
    return this.ast.toString().replace(/,\n/g, ',');
  }

  return '';
}
```
- example usage
```shell
...
    this.readRules(rule.rules);
  }
}.bind(this));
};

CssTreeWalker.prototype.toString = function () {
if (this.ast) {
  return this.ast.toString().replace(/,\n/g, ',');
}

return '';
};

CssTreeWalker.prototype.removeEmptyRules = function (rules) {
var emptyRules = [];
...
```



# <a name="apidoc.module.purify-css.SelectorFilter"></a>[module purify-css.SelectorFilter](#apidoc.module.purify-css.SelectorFilter)

#### <a name="apidoc.element.purify-css.SelectorFilter.SelectorFilter"></a>[function <span class="apidocSignatureSpan">purify-css.</span>SelectorFilter (contentWords, whitelist)](#apidoc.element.purify-css.SelectorFilter.SelectorFilter)
- description and source-code
```javascript
SelectorFilter = function (contentWords, whitelist) {
  this.contentWords = contentWords;
  this.rejectedSelectors = [];
  this.wildcardWhitelist = [];

  this.parseWhitelist(whitelist);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.purify-css.SelectorFilter.prototype"></a>[module purify-css.SelectorFilter.prototype](#apidoc.module.purify-css.SelectorFilter.prototype)

#### <a name="apidoc.element.purify-css.SelectorFilter.prototype.filterSelectors"></a>[function <span class="apidocSignatureSpan">purify-css.SelectorFilter.prototype.</span>filterSelectors (selectors)](#apidoc.element.purify-css.SelectorFilter.prototype.filterSelectors)
- description and source-code
```javascript
filterSelectors = function (selectors) {
  var contentWords = this.contentWords;
  var rejectedSelectors = this.rejectedSelectors;
  var wildcardWhitelist = this.wildcardWhitelist;
  var usedSelectors = [];

  selectors.forEach(function (selector) {
    if (hasWhitelistMatch(selector, wildcardWhitelist)) {
      usedSelectors.push(selector);
      return;
    }

    var words = getAllWordsInSelector(selector);
    var usedWords = words.filter(function (word) {
      return contentWords[word];
    });

    if (usedWords.length === words.length) {
      usedSelectors.push(selector);
    } else {
      rejectedSelectors.push(selector);
    }
  });

  return usedSelectors;
}
```
- example usage
```shell
...
      this.contentWords[word] = true;
    }.bind(this));
  }
}.bind(this));
};

SelectorFilter.prototype.parseRule = function (selectors, rule) {
rule.selectors = this.filterSelectors(selectors);
};

SelectorFilter.prototype.filterSelectors = function (selectors) {
var contentWords = this.contentWords;
var rejectedSelectors = this.rejectedSelectors;
var wildcardWhitelist = this.wildcardWhitelist;
var usedSelectors = [];
...
```

#### <a name="apidoc.element.purify-css.SelectorFilter.prototype.initialize"></a>[function <span class="apidocSignatureSpan">purify-css.SelectorFilter.prototype.</span>initialize (CssSyntaxTree)](#apidoc.element.purify-css.SelectorFilter.prototype.initialize)
- description and source-code
```javascript
initialize = function (CssSyntaxTree) {
  CssSyntaxTree.on('readRule', this.parseRule.bind(this));
}
```
- example usage
```shell
...

var CssTreeWalker = function (code, plugins) {
  EventEmitter.call(this);
  this.startingSource = code;
  this.ast = null;

  plugins.forEach(function (plugin) {
    plugin.initialize(this);
  }.bind(this));
};

CssTreeWalker.prototype = Object.create(EventEmitter.prototype);
CssTreeWalker.prototype.constructor = CssTreeWalker;

CssTreeWalker.prototype.beginReading = function () {
...
```

#### <a name="apidoc.element.purify-css.SelectorFilter.prototype.parseRule"></a>[function <span class="apidocSignatureSpan">purify-css.SelectorFilter.prototype.</span>parseRule (selectors, rule)](#apidoc.element.purify-css.SelectorFilter.prototype.parseRule)
- description and source-code
```javascript
parseRule = function (selectors, rule) {
  rule.selectors = this.filterSelectors(selectors);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.purify-css.SelectorFilter.prototype.parseWhitelist"></a>[function <span class="apidocSignatureSpan">purify-css.SelectorFilter.prototype.</span>parseWhitelist (whitelist)](#apidoc.element.purify-css.SelectorFilter.prototype.parseWhitelist)
- description and source-code
```javascript
parseWhitelist = function (whitelist) {
  whitelist.forEach(function (whitelistSelector) {
    whitelistSelector = whitelistSelector.toLowerCase();

    if (isWildcardWhitelistSelector(whitelistSelector)) {
      // If '*button*' then push 'button' onto list.
      this.wildcardWhitelist.push(
        whitelistSelector.substr(1, whitelistSelector.length - 2)
      );
    } else {
      getAllWordsInSelector(whitelistSelector).forEach(function (word) {
        this.contentWords[word] = true;
      }.bind(this));
    }
  }.bind(this));
}
```
- example usage
```shell
...
}

var SelectorFilter = function (contentWords, whitelist) {
  this.contentWords = contentWords;
  this.rejectedSelectors = [];
  this.wildcardWhitelist = [];

  this.parseWhitelist(whitelist);
};

SelectorFilter.prototype.initialize = function (CssSyntaxTree) {
  CssSyntaxTree.on('readRule', this.parseRule.bind(this));
};

SelectorFilter.prototype.parseWhitelist = function (whitelist) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
