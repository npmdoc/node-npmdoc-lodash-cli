# api documentation for  [lodash-cli (v4.17.4)](https://lodash.com/custom-builds)  [![npm package](https://img.shields.io/npm/v/npmdoc-lodash-cli.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-lodash-cli) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-lodash-cli.svg)](https://travis-ci.org/npmdoc/node-npmdoc-lodash-cli)
#### The Lodash command-line interface.

[![NPM](https://nodei.co/npm/lodash-cli.png?downloads=true)](https://www.npmjs.com/package/lodash-cli)

[![apidoc](https://npmdoc.github.io/node-npmdoc-lodash-cli/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-lodash-cli_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-lodash-cli/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-lodash-cli/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-lodash-cli/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "John-David Dalton",
        "email": "john.david.dalton@gmail.com",
        "url": "http://allyoucanleet.com/"
    },
    "bin": {
        "lodash": "bin/lodash"
    },
    "bugs": {
        "url": "https://github.com/lodash/lodash-cli/issues"
    },
    "contributors": [
        {
            "name": "John-David Dalton",
            "email": "john.david.dalton@gmail.com",
            "url": "http://allyoucanleet.com/"
        },
        {
            "name": "Mathias Bynens",
            "email": "mathias@qiwi.be",
            "url": "https://mathiasbynens.be/"
        }
    ],
    "dependencies": {
        "closure-compiler": "0.2.12",
        "glob": "7.1.1",
        "lodash": "4.17.4",
        "semver": "5.3.0",
        "uglify-js": "2.7.5"
    },
    "description": "The Lodash command-line interface.",
    "devDependencies": {
        "babel-cli": "^6.18.0",
        "babel-preset-env": "^1.1.4",
        "qunit-extras": "^3.0.0",
        "qunitjs": "^2.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "23b727cd0e91e28484fafda1521900a8a811df81",
        "tarball": "https://registry.npmjs.org/lodash-cli/-/lodash-cli-4.17.4.tgz"
    },
    "files": [
        "bin",
        "lib",
        "template",
        "npm-shrinkwrap.json"
    ],
    "greenkeeper": {
        "ignore": [
            "lodash"
        ]
    },
    "homepage": "https://lodash.com/custom-builds",
    "keywords": [
        "builder",
        "compile",
        "customize",
        "lodash"
    ],
    "license": "MIT",
    "main": "bin/lodash",
    "maintainers": [
        {
            "name": "jdalton",
            "email": "john.david.dalton@gmail.com"
        },
        {
            "name": "mathias",
            "email": "mathias@qiwi.be"
        }
    ],
    "name": "lodash-cli",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/lodash/lodash-cli.git"
    },
    "scripts": {
        "test": "node test"
    },
    "version": "4.17.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module lodash-cli](#apidoc.module.lodash-cli)
1.  object <span class="apidocSignatureSpan">lodash-cli.</span>util

#### [module lodash-cli.util](#apidoc.module.lodash-cli.util)
1.  [function <span class="apidocSignatureSpan">lodash-cli.util.</span>Hash (properties)](#apidoc.element.lodash-cli.util.Hash)
1.  object <span class="apidocSignatureSpan">lodash-cli.util.</span>fs
1.  object <span class="apidocSignatureSpan">lodash-cli.util.</span>path



# <a name="apidoc.module.lodash-cli"></a>[module lodash-cli](#apidoc.module.lodash-cli)



# <a name="apidoc.module.lodash-cli.util"></a>[module lodash-cli.util](#apidoc.module.lodash-cli.util)

#### <a name="apidoc.element.lodash-cli.util.Hash"></a>[function <span class="apidocSignatureSpan">lodash-cli.util.</span>Hash (properties)](#apidoc.element.lodash-cli.util.Hash)
- description and source-code
```javascript
function Hash(properties) {
  return _.transform(properties, function(result, value, key) {
    result[key] = (_.isPlainObject(value) && !(value instanceof Hash))
      ? new Hash(value)
      : value;
  }, this);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
