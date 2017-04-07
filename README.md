# api documentation for  [flatpickr (v2.4.8)](https://chmln.github.io/flatpickr)  [![npm package](https://img.shields.io/npm/v/npmdoc-flatpickr.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-flatpickr) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-flatpickr.svg)](https://travis-ci.org/npmdoc/node-npmdoc-flatpickr)
#### A lightweight, powerful javascript datetime picker

[![NPM](https://nodei.co/npm/flatpickr.png?downloads=true)](https://www.npmjs.com/package/flatpickr)

[![apidoc](https://npmdoc.github.io/node-npmdoc-flatpickr/build/screenCapture.buildNpmdoc.browser.%2Fhome%2Ftravis%2Fbuild%2Fnpmdoc%2Fnode-npmdoc-flatpickr%2Ftmp%2Fbuild%2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-flatpickr/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-flatpickr/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-flatpickr/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Gregory",
        "email": "gregory.mkv@gmail.com"
    },
    "bugs": {
        "url": "https://github.com/chmln/flatpickr/issues"
    },
    "collective": {
        "type": "opencollective",
        "url": "https://opencollective.com/flatpickr",
        "logo": "https://opencollective.com/opencollective/logo.txt"
    },
    "dependencies": {},
    "description": "A lightweight, powerful javascript datetime picker",
    "devDependencies": {
        "babel-cli": "^6.24.0",
        "babel-plugin-transform-object-assign": "^6.22.0",
        "babel-plugin-transform-remove-strict-mode": "0.0.2",
        "babel-preset-es2015": "^6.24.0",
        "coveralls": "^2.12.0",
        "eslint": "^3.18.0",
        "http-server": "^0.9.0",
        "jest": "^19.0.2",
        "livereload": "^0.6.2",
        "ncp": "^2.0.0",
        "npm-run-all": "^4.0.2",
        "onchange": "^3.2.1",
        "opencollective-postinstall": "^1.0.14",
        "rtlcss": "^2.1.2",
        "semver": "^5.3.0",
        "stylus": "^0.54.5",
        "uglify-js": "^2.8.16"
    },
    "directories": {},
    "dist": {
        "shasum": "152136c6657089ebb7c6af8cd969054c55bd3dd4",
        "tarball": "https://registry.npmjs.org/flatpickr/-/flatpickr-2.4.8.tgz"
    },
    "gitHead": "57b30d591d23875bc6058a070e8cf3af2da94cf3",
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
    "license": "MIT",
    "main": "dist/flatpickr.js",
    "maintainers": [
        {
            "name": "chmln",
            "email": "gregory.mkv@gmail.com"
        }
    ],
    "name": "flatpickr",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/chmln/flatpickr.git"
    },
    "scripts": {
        "build": "run-p build:*",
        "build:extra": "run-p build:extra:*",
        "build:extra:l10n": "babel src/l10n --out-dir dist/l10n",
        "build:extra:plugins": "ncp src/plugins dist/plugins && babel src/plugins --out-dir dist/plugins",
        "build:script": "run-s build:script:unmin build:script:min",
        "build:script:min": " uglifyjs -c -m --comments -o dist/flatpickr.min.js -- dist/flatpickr.js ",
        "build:script:unmin": "babel src/flatpickr.js --out-file dist/flatpickr.js",
        "build:style": "run-p build:style:*",
        "build:style:min": "stylus -c < ./src/style/flatpickr.styl > dist/flatpickr.min.css",
        "build:style:rtl": "rtlcss -d ./dist/themes ./dist/rtl/themes && rtlcss dist/flatpickr.min.css dist/rtl/flatpickr.min.css",
        "build:style:themes": "stylus --out dist/themes src/style/themes",
        "build:style:unmin": "stylus < ./src/style/flatpickr.styl > dist/flatpickr.css",
        "coveralls": "jest --coverage && cat ./coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js",
        "dev": "run-p dev:*",
        "dev:plugins": "onchange \"src/plugins/**/*\" -- run-s build:extra:plugins",
        "dev:script": "onchange \"src/flatpickr.js\" -- run-s lint build:script:unmin",
        "dev:style": "onchange \"src/style/**/*\" -- run-p build:style:unmin build:style:themes",
        "lint": "eslint src/flatpickr.js || (exit 0)",
        "release": "jest --bail --silent && ./release",
        "serve": "run-p serve:*",
        "serve:http": "http-server -o --silent",
        "serve:livereload": "livereload \"dist\"",
        "start": "run-p build dev serve lint",
        "test": "jest --bail"
    },
    "style": "dist/flatpickr.css",
    "version": "2.4.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module flatpickr](#apidoc.module.flatpickr)



# <a name="apidoc.module.flatpickr"></a>[module flatpickr](#apidoc.module.flatpickr)



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
