# npmtest-levelgraph

#### basic test coverage for  levelgraph (v2.0.1)  [![npm package](https://img.shields.io/npm/v/npmtest-levelgraph.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-levelgraph) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-levelgraph.svg)](https://travis-ci.org/npmtest/node-npmtest-levelgraph)

#### A graph database for Node.js and the browser built on top of LevelUp

[![NPM](https://nodei.co/npm/levelgraph.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/levelgraph)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-levelgraph/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-levelgraph/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-levelgraph/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-levelgraph/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-levelgraph/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-levelgraph/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-levelgraph/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-levelgraph/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-levelgraph/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-levelgraph/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-levelgraph/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-levelgraph/build/test-report.html](https://npmtest.github.io/node-npmtest-levelgraph/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-levelgraph/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-levelgraph/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-levelgraph/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-levelgraph/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-levelgraph/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-levelgraph/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-levelgraph/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-levelgraph/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "levelgraph",
    "version": "2.0.1",
    "description": "A graph database for Node.js and the browser built on top of LevelUp",
    "main": "lib/levelgraph.js",
    "scripts": {
        "test": "mocha --recursive --bail --reporter spec test",
        "zuul": "zuul test/common.js test/*spec.js",
        "zuul-local": "zuul --open --local 8080 -- test/common.js test/*spec.js",
        "coverage": "rm -rf coverage; istanbul cover _mocha -- --recursive --reporter spec --bail",
        "publish-coverage": "cat coverage/lcov.info | coveralls",
        "ci": "mocha --recursive --bail --watch test",
        "jshint-lib": "jshint lib/*.js",
        "jshint-test": "jshint test/*.js"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/mcollina/levelgraph.git"
    },
    "bugs": {
        "url": "http://github.com/mcollina/levelgraph/issues"
    },
    "pre-commit": [
        "jshint-lib",
        "jshint-test",
        "test"
    ],
    "keywords": [
        "leveldb",
        "graph",
        "level",
        "database",
        "triples",
        "triple"
    ],
    "author": "Matteo Collina <hello@matteocollina.com>",
    "license": "MIT",
    "devDependencies": {
        "browserify": "^13.0.1",
        "chai": "^3.5.0",
        "coveralls": "^2.11.2",
        "istanbul": "~0.4.3",
        "jshint": "^2.9.2",
        "level-browserify": "^1.0.1",
        "level-sublevel": "^6.4.6",
        "memdb": "^1.3.1",
        "mocha": "^3.0.0",
        "multilevel": "^7.2.0",
        "osenv": "^0.1.0",
        "pre-commit": "^1.1.3",
        "setimmediate": "^1.0.2",
        "sinon": "~1.17.4",
        "sinon-chai": "^2.6.0",
        "uglify-js": "^2.6.2",
        "zuul": "^3.0.0"
    },
    "dependencies": {
        "callback-stream": "^1.1.0",
        "inherits": "^2.0.1",
        "level-ws": "0.0.1",
        "lodash.keys": "^4.0.6",
        "pump": "^1.0.1",
        "readable-stream": "^2.0.0",
        "steed": "^1.1.3",
        "xtend": "~4.0.0"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
