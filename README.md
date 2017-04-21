# npmtest-angular-in-memory-web-api

#### basic test coverage for  [angular-in-memory-web-api (v0.3.1)](https://github.com/angular/in-memory-web-api#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-angular-in-memory-web-api.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-angular-in-memory-web-api) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-angular-in-memory-web-api.svg)](https://travis-ci.org/npmtest/node-npmtest-angular-in-memory-web-api)

#### An in-memory web api for Angular demos and tests

[![NPM](https://nodei.co/npm/angular-in-memory-web-api.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/angular-in-memory-web-api)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-angular-in-memory-web-api/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-angular-in-memory-web-api/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/test-report.html](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-angular-in-memory-web-api/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-angular-in-memory-web-api/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-angular-in-memory-web-api/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-angular-in-memory-web-api/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-angular-in-memory-web-api/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "angular-in-memory-web-api",
    "version": "0.3.1",
    "description": "An in-memory web api for Angular demos and tests",
    "main": "bundles/in-memory-web-api.umd.js",
    "module": "index.js",
    "scripts": {
        "tsc": "tsc",
        "ngc": "ngc",
        "tsc:w": "tsc -w",
        "lint": "tslint ./src/*.ts -t verbose -e ./src/*.d.ts",
        "lite": "lite-server",
        "live": "live-server",
        "start": "concurrently \"npm run tsc:w\" \"npm run lite\" ",
        "test": "karma start karma.conf.js",
        "build-and-test": "concurrently  \"npm run tsc\" \"npm run test\"",
        "http-server": "tsc && http-server"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/angular/in-memory-web-api.git"
    },
    "keywords": [],
    "author": "",
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/angular/in-memory-web-api/issues"
    },
    "homepage": "https://github.com/angular/in-memory-web-api#readme",
    "peerDependencies": {
        "@angular/core": ">=2.0.0 <5.0.0 || >=4.0.0-beta <5.0.0",
        "@angular/http": ">=2.0.0 <5.0.0 || >=4.0.0-beta <5.0.0",
        "rxjs": "^5.0.1"
    },
    "devDependencies": {
        "@angular/common": "~2.4.0",
        "@angular/compiler": "~2.4.0",
        "@angular/compiler-cli": "~2.4.0",
        "@angular/core": "~2.4.0",
        "@angular/http": "~2.4.0",
        "@angular/platform-browser": "~2.4.0",
        "@angular/platform-server": "~2.4.0",
        "@types/jasmine": "2.5.36",
        "@types/node": "^6.0.46",
        "canonical-path": "0.0.2",
        "concurrently": "^3.0.0",
        "core-js": "^2.4.1",
        "del": "^2.2.2",
        "gulp": "^3.9.1",
        "gulp-bump": "^2.4.0",
        "gulp-load-plugins": "^1.3.0",
        "gulp-task-listing": "^1.0.1",
        "gulp-util": "^3.0.7",
        "http-server": "^0.9.0",
        "jasmine-core": "~2.5.2",
        "karma": "^1.3.0",
        "karma-chrome-launcher": "^2.0.0",
        "karma-cli": "^1.0.1",
        "karma-htmlfile-reporter": "^0.3.4",
        "karma-jasmine": "^1.0.2",
        "karma-jasmine-html-reporter": "^0.2.2",
        "lite-server": "^2.2.2",
        "lodash": "^4.16.2",
        "rimraf": "^2.5.4",
        "rollup": "^0.36.0",
        "rollup-stream": "^1.14.0",
        "rxjs": "^5.0.1",
        "tslint": "^3.15.1",
        "typescript": "~2.0.10",
        "vinyl-source-stream": "^1.1.0",
        "yargs": "^5.0.0",
        "zone.js": "^0.7.2"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
