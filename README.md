# npmdoc-loggly

#### api documentation for  [loggly (v1.1.1)](https://github.com/winstonjs/node-loggly#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-loggly.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-loggly) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-loggly.svg)](https://travis-ci.org/npmdoc/node-npmdoc-loggly)

#### A client implementation for Loggly cloud Logging-as-a-Service API

[![NPM](https://nodei.co/npm/loggly.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/loggly)

- [https://npmdoc.github.io/node-npmdoc-loggly/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-loggly/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-loggly/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-loggly/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-loggly/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-loggly/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Charlie Robbins"
    },
    "bugs": {
        "url": "https://github.com/winstonjs/node-loggly/issues"
    },
    "dependencies": {
        "json-stringify-safe": "5.0.x",
        "request": "2.75.x",
        "timespan": "2.3.x"
    },
    "description": "A client implementation for Loggly cloud Logging-as-a-Service API",
    "devDependencies": {
        "common-style": "^3.1.0",
        "vows": "0.8.x"
    },
    "directories": {},
    "dist": {
        "shasum": "0a0fc1d3fa3a5ec44fdc7b897beba2a4695cebee",
        "tarball": "https://registry.npmjs.org/loggly/-/loggly-1.1.1.tgz"
    },
    "engines": {
        "node": ">= 0.8.0"
    },
    "gitHead": "34c562bcb584b42cab4298c30151707ab5788137",
    "homepage": "https://github.com/winstonjs/node-loggly#readme",
    "keywords": [
        "cloud computing",
        "api",
        "logging",
        "loggly"
    ],
    "license": "MIT",
    "main": "./lib/loggly",
    "maintainers": [
        {
            "name": "indexzero"
        },
        {
            "name": "jcrugzz"
        }
    ],
    "name": "loggly",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/winstonjs/node-loggly.git"
    },
    "scripts": {
        "pretest": "common lib/**/*.js lib/*.js test/helpers.js",
        "test": "vows test/*-test.js --spec"
    },
    "version": "1.1.1"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
