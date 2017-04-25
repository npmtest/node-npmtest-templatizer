# npmtest-templatizer

#### basic test coverage for  [templatizer (v2.0.5)](https://github.com/HenrikJoreteg/templatizer)  [![npm package](https://img.shields.io/npm/v/npmtest-templatizer.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-templatizer) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-templatizer.svg)](https://travis-ci.org/npmtest/node-npmtest-templatizer)

#### Simple solution for compiling jade templates into vanilla JS functions for blazin' fast client-side use.

[![NPM](https://nodei.co/npm/templatizer.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/templatizer)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-templatizer/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-templatizer/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-templatizer/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-templatizer/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-templatizer/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-templatizer/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-templatizer/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-templatizer/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-templatizer/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-templatizer/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-templatizer/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-templatizer/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-templatizer/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-templatizer/build/test-report.html](https://npmtest.github.io/node-npmtest-templatizer/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-templatizer/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-templatizer/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-templatizer/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-templatizer/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-templatizer/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-templatizer/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-templatizer/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-templatizer/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Henrik Joreteg"
    },
    "bin": {
        "templatizer": "./bin/cli"
    },
    "bugs": {
        "url": "https://github.com/HenrikJoreteg/templatizer/issues"
    },
    "contributors": [
        {
            "name": "Beau Sorensen"
        },
        {
            "name": "Luke Karrys"
        }
    ],
    "dependencies": {
        "async": "^1.4.2",
        "escodegen": "1.6.1",
        "esprima": "^2.5.0",
        "falafel": "^1.2.0",
        "glob": "^5.0.14",
        "jade": "^1.11.0",
        "lodash": "^3.10.1",
        "minimatch": "^2.0.10",
        "minimist": "^1.1.3",
        "uglify-js": "^2.4.24",
        "walkdir": "0.0.10"
    },
    "description": "Simple solution for compiling jade templates into vanilla JS functions for blazin' fast client-side use.",
    "devDependencies": {
        "@lukekarrys/jade-runtime": "^1.11.1",
        "browserify": "^11.0.1",
        "colors": "^1.1.2",
        "http-server": "^0.8.0",
        "jshint": "^2.8.0",
        "mkdirp": "^0.5.1",
        "phantomjs": "^1.9.7-15",
        "precommit-hook": "^3.0.0",
        "rimraf": "^2.4.2",
        "run-browser": "^2.0.2",
        "tap-spec": "^4.0.2",
        "tape": "^4.2.0",
        "tape-run": "^1.1.0",
        "underscore": "^1.8.3",
        "yetify": "0.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "dafab6d9ecf824571b040fdfce1f0745f982317d",
        "tarball": "https://registry.npmjs.org/templatizer/-/templatizer-2.0.5.tgz"
    },
    "gitHead": "62f831153464b37979d8c7152d748604b34cd304",
    "homepage": "https://github.com/HenrikJoreteg/templatizer",
    "keywords": [
        "browser",
        "jade",
        "templates"
    ],
    "license": "MIT",
    "main": "templatizer.js",
    "maintainers": [
        {
            "name": "andyet-ops"
        },
        {
            "name": "henrikjoreteg"
        },
        {
            "name": "lukekarrys"
        }
    ],
    "name": "templatizer",
    "optionalDependencies": {},
    "peerDependencies": {
        "@lukekarrys/jade-runtime": "^1.11.1"
    },
    "pre-commit": [
        "lint",
        "validate",
        "test"
    ],
    "repository": {
        "type": "git",
        "url": "git+https://github.com/HenrikJoreteg/templatizer.git"
    },
    "scripts": {
        "benchmark": "node benchmark/speedtest.js",
        "lint": "jshint .",
        "start": "run-browser test/index.js",
        "test": "node test/build && browserify test/index.js | tape-run -b phantom | tap-spec",
        "validate": "npm ls"
    },
    "version": "2.0.5"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
