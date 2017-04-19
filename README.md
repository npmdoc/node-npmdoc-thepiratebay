# npmdoc-thepiratebay

#### api documentation for  [thepiratebay (v1.4.0)](http://github.com/t3chnoboy/thepiratebay)  [![npm package](https://img.shields.io/npm/v/npmdoc-thepiratebay.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-thepiratebay) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-thepiratebay.svg)](https://travis-ci.org/npmdoc/node-npmdoc-thepiratebay)

#### The pirate bay client

[![NPM](https://nodei.co/npm/thepiratebay.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/thepiratebay)

- [https://npmdoc.github.io/node-npmdoc-thepiratebay/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-thepiratebay/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-thepiratebay/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-thepiratebay/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-thepiratebay/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-thepiratebay/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dmitry Mazuro"
    },
    "bugs": {
        "url": "https://github.com/t3chnoboy/thepiratebay/issues"
    },
    "dependencies": {
        "babel-runtime": "^6.23.0",
        "cheerio": "^0.22.0",
        "form-data": "^2.1.2",
        "isomorphic-fetch": "^2.2.1",
        "url-parse": "^1.1.8"
    },
    "description": "The pirate bay client",
    "devDependencies": {
        "babel-cli": "^6.24.0",
        "babel-eslint": "^7.2.1",
        "babel-loader": "^6.4.1",
        "babel-plugin-add-module-exports": "^0.2.1",
        "babel-plugin-transform-es2015-modules-umd": "^6.24.0",
        "babel-plugin-transform-flow-strip-types": "^6.22.0",
        "babel-plugin-transform-runtime": "^6.23.0",
        "babel-polyfill": "^6.23.0",
        "babel-preset-es2015": "^6.24.0",
        "babel-preset-latest": "^6.24.0",
        "babel-preset-stage-0": "^6.22.0",
        "babel-register": "^6.24.0",
        "chai": "^3.5.0",
        "cross-env": "^3.2.4",
        "eslint": "^3.18.0",
        "eslint-config-bliss": "^1.0.3",
        "eslint-formatter-pretty": "^1.1.0",
        "flow-bin": "^0.42.0",
        "flow-typed": "^2.0.0",
        "jest-cli": "^19.0.2",
        "json-loader": "^0.5.4"
    },
    "devEngines": {
        "node": ">=4.x",
        "npm": ">=3.x"
    },
    "directories": {},
    "dist": {
        "shasum": "e5e12468928bcea517cdd361a38282ef242b709e",
        "tarball": "https://registry.npmjs.org/thepiratebay/-/thepiratebay-1.4.0.tgz"
    },
    "engines": {
        "node": ">=4.x",
        "npm": ">=3.x"
    },
    "files": [
        "lib"
    ],
    "gitHead": "d7bf9b539614cc0572b00273dd8c45b49ade2613",
    "homepage": "http://github.com/t3chnoboy/thepiratebay",
    "jest": {
        "testEnvironment": "node"
    },
    "keywords": [
        "thepiratebay",
        "pirate bay",
        "torrent",
        "api",
        "client",
        "scraper"
    ],
    "license": "MIT",
    "main": "./lib/PirateBay.js",
    "maintainers": [
        {
            "name": "t3chnoboy"
        },
        {
            "name": "redbackthomson"
        }
    ],
    "name": "thepiratebay",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/t3chnoboy/thepiratebay.git"
    },
    "scripts": {
        "build": "cross-env NODE_ENV=production babel src --out-dir lib",
        "clean": "rm -rf lib",
        "flow": "flow check",
        "flow-typed": "flow-typed install",
        "lint": "eslint --cache --format=node_modules/eslint-formatter-pretty .",
        "spec": "jest",
        "test": "cross-env NODE_ENV=test npm run lint && npm run spec && npm run build",
        "version": "npm run build"
    },
    "version": "1.4.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
