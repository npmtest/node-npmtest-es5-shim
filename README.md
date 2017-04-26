# npmtest-es5-shim

#### basic test coverage for  [es5-shim (v4.5.9)](http://github.com/es-shims/es5-shim/)  [![npm package](https://img.shields.io/npm/v/npmtest-es5-shim.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-es5-shim) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-es5-shim.svg)](https://travis-ci.org/npmtest/node-npmtest-es5-shim)

#### ECMAScript 5 compatibility shims for legacy JavaScript engines

[![NPM](https://nodei.co/npm/es5-shim.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/es5-shim)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-es5-shim/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-es5-shim/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-es5-shim/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-es5-shim/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-es5-shim/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-es5-shim/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-es5-shim/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-es5-shim/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-es5-shim/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-es5-shim/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-es5-shim/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-es5-shim/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-es5-shim/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-es5-shim/build/test-report.html](https://npmtest.github.io/node-npmtest-es5-shim/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-es5-shim/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-es5-shim/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-es5-shim/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-es5-shim/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-es5-shim/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-es5-shim/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-es5-shim/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-es5-shim/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "bugs": {
        "url": "http://github.com/es-shims/es5-shim/issues"
    },
    "contributors": [
        {
            "name": "Kris Kowal",
            "url": "http://github.com/kriskowal/"
        },
        {
            "name": "Sami Samhuri",
            "url": "http://samhuri.net/"
        },
        {
            "name": "Florian Schäfer",
            "url": "http://github.com/fschaefer"
        },
        {
            "name": "Irakli Gozalishvili",
            "url": "http://jeditoolkit.com"
        },
        {
            "name": "Kit Cambridge",
            "url": "http://kitcambridge.github.com"
        },
        {
            "name": "Jordan Harband",
            "url": "https://github.com/ljharb/"
        }
    ],
    "dependencies": {},
    "description": "ECMAScript 5 compatibility shims for legacy JavaScript engines",
    "devDependencies": {
        "@ljharb/eslint-config": "^5.0.0",
        "concurrently": "^2.1.0",
        "eslint": "^2.12.0",
        "jasmine-node": "^1.14.5",
        "jscs": "^3.0.4",
        "replace": "^0.3.0",
        "semver": "^5.1.0",
        "uglify-js": "^2.6.2"
    },
    "directories": {},
    "dist": {
        "shasum": "2a1e2b9e583ff5fed0c20a3ee2cbf3f75230a5c0",
        "tarball": "https://registry.npmjs.org/es5-shim/-/es5-shim-4.5.9.tgz"
    },
    "engines": {
        "node": ">=0.4.0"
    },
    "gitHead": "30ebdda82ed0d8f42b05785debf1e7ee066c3507",
    "homepage": "http://github.com/es-shims/es5-shim/",
    "keywords": [
        "shim",
        "es5",
        "es5 shim",
        "javascript",
        "ecmascript",
        "polyfill"
    ],
    "license": "MIT",
    "main": "es5-shim.js",
    "maintainers": [
        {
            "name": "kriskowal"
        },
        {
            "name": "gozala"
        },
        {
            "name": "ljharb"
        }
    ],
    "name": "es5-shim",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/es-shims/es5-shim.git"
    },
    "scripts": {
        "eslint": "eslint tests/helpers/*.js tests/spec/*.js es5-shim.js es5-sham.js",
        "jscs": "jscs tests/helpers/*.js tests/spec/*.js es5-shim.js es5-sham.js",
        "lint": "concurrently --raw 'npm run --silent jscs' 'npm run --silent eslint'",
        "minify": "concurrently --raw 'npm run --silent minify-shim' 'npm run --silent minify-sham'",
        "minify-sham": "uglifyjs es5-sham.js --keep-fnames --comments --source-map=es5-sham.map -m -b ascii_only=true,beautify=false > es5-sham.min.js",
        "minify-shim": "uglifyjs es5-shim.js --keep-fnames --comments --source-map=es5-shim.map -m -b ascii_only=true,beautify=false > es5-shim.min.js",
        "pretest": "npm run --silent lint",
        "test": "npm run --silent tests-only",
        "test-native": "jasmine-node --matchall tests/spec/",
        "tests-only": "jasmine-node --matchall ./ tests/spec/"
    },
    "testling": {
        "browsers": [
            "iexplore/6.0..latest",
            "firefox/3.0..6.0",
            "firefox/18.0..latest",
            "firefox/nightly",
            "chrome/4.0..10.0",
            "chrome/25.0..latest",
            "chrome/canary",
            "opera/10.0..latest",
            "opera/next",
            "safari/4.0..latest",
            "ipad/6.0..latest",
            "iphone/6.0..latest",
            "android-browser/4.2"
        ]
    },
    "version": "4.5.9",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
