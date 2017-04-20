# npmdoc-firmata

#### api documentation for  [firmata (v0.16.0)](http://www.github.com/firmata/firmata.js)  [![npm package](https://img.shields.io/npm/v/npmdoc-firmata.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-firmata) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-firmata.svg)](https://travis-ci.org/npmdoc/node-npmdoc-firmata)

#### Firmata protocol implementation for programmatic interaction with Arduino and Arduino compatible development boards.

[![NPM](https://nodei.co/npm/firmata.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/firmata)

- [https://npmdoc.github.io/node-npmdoc-firmata/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-firmata/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-firmata/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-firmata/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-firmata/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-firmata/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "firmata",
    "description": "Firmata protocol implementation for programmatic interaction with Arduino and Arduino compatible development boards.",
    "version": "0.16.0",
    "author": "Julian Gautier",
    "license": "MIT",
    "homepage": "http://www.github.com/firmata/firmata.js",
    "repository": {
        "type": "git",
        "url": "git://github.com/firmata/firmata.js.git"
    },
    "main": "lib/firmata",
    "bin": {
        "firmata": "./repl.js"
    },
    "devDependencies": {
        "browserify": "^13.0.0",
        "common-tags": "^1.4.0",
        "coveralls": "^2.11.15",
        "grunt": "^1.0.1",
        "grunt-cli": "^1.2.0",
        "grunt-contrib-jshint": "^1.0.0",
        "grunt-jsbeautifier": "~0.2.13",
        "grunt-jscs": "^3.0.1",
        "grunt-mocha-test": "~0.12.7",
        "mocha": "^2.3.x",
        "nyc": "^10.0.0",
        "should": "^7.1.x",
        "sinon": "~1.17.1",
        "webpack": "^1.12.14"
    },
    "dependencies": {
        "browser-serialport": "latest",
        "es6-shim": "latest",
        "serialport": "^4.0.0"
    },
    "scripts": {
        "test": "grunt",
        "attempt-timeout": "node examples/test-i2c-read.js && node examples/test-i2c-read.js && node examples/test-analog-read.js && node examples/test-analog-read.js && node examples/test-serial-read.js && node examples/test-serial-read.js",
        "test-cover": "nyc grunt test",
        "coveralls": "nyc --reporter=lcov grunt test && cat ./coverage/lcov.info | coveralls"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
