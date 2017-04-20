# npmdoc-flatpickr

#### api documentation for  [flatpickr (v2.5.7)](https://chmln.github.io/flatpickr)  [![npm package](https://img.shields.io/npm/v/npmdoc-flatpickr.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-flatpickr) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-flatpickr.svg)](https://travis-ci.org/npmdoc/node-npmdoc-flatpickr)

#### A lightweight, powerful javascript datetime picker

[![NPM](https://nodei.co/npm/flatpickr.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/flatpickr)

- [https://npmdoc.github.io/node-npmdoc-flatpickr/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-flatpickr/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-flatpickr/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-flatpickr/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-flatpickr/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-flatpickr/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "flatpickr",
    "version": "2.5.7",
    "description": "A lightweight, powerful javascript datetime picker",
    "scripts": {
        "start": "nodemon --watch build.js build.js -- --dev",
        "build": "node build.js",
        "test": "jest --bail",
        "coveralls": "jest --coverage && cat ./coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js",
        "release": "jest --bail --silent && ./release"
    },
    "dependencies": {},
    "devDependencies": {
        "autoprefixer-stylus": "^0.13.0",
        "babel-cli": "next",
        "babel-plugin-transform-object-assign": "next",
        "babel-plugin-transform-remove-strict-mode": "latest",
        "babel-preset-es2015": "next",
        "chokidar": "^1.6.1",
        "coveralls": "latest",
        "eslint": "latest",
        "glob": "^7.1.1",
        "http-server": "latest",
        "jest": "latest",
        "livereload": "latest",
        "ncp": "latest",
        "node-watch": "^0.5.2",
        "nodemon": "^1.11.0",
        "npm-run-all": "latest",
        "opn": "^4.0.2",
        "rtlcss": "latest",
        "semver": "latest",
        "stylus": "latest",
        "uglify-js": "latest"
    },
    "main": "dist/flatpickr.js",
    "style": "dist/flatpickr.css",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/chmln/flatpickr.git"
    },
    "author": "Gregory <gregory.mkv@gmail.com>",
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/chmln/flatpickr/issues"
    },
    "homepage": "https://chmln.github.io/flatpickr",
    "keywords": [
        "javascript",
        "datetimepicker",
        "calendar",
        "date",
        "time",
        "picker",
        "lightweight"
    ],
    "collective": {
        "type": "opencollective",
        "url": "https://opencollective.com/flatpickr",
        "logo": "https://opencollective.com/opencollective/logo.txt"
    },
    "browserslist": [
        "ie >= 9",
        "last 2 versions",
        "safari >= 7"
    ]
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
