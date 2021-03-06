# npmdoc-better-npm-run

#### basic api documentation for  [better-npm-run (v0.0.15)](https://github.com/benoror/better-npm-run#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-better-npm-run.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-better-npm-run) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-better-npm-run.svg)](https://travis-ci.org/npmdoc/node-npmdoc-better-npm-run)

#### Better NPM scripts runner

[![NPM](https://nodei.co/npm/better-npm-run.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/better-npm-run)

- [https://npmdoc.github.io/node-npmdoc-better-npm-run/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-better-npm-run/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-better-npm-run/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-better-npm-run/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-better-npm-run/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-better-npm-run/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Benjamin Orozco"
    },
    "betterScripts": {
        "test:command:string": "node ./test/command.js",
        "test:command:object": {
            "command": "node ./test/command.js"
        },
        "test:params": {
            "command": "node ./test/params.js"
        },
        "test:env": {
            "command": "node ./test/env.js",
            "env": {
                "FOO": "bar"
            }
        },
        "test:env-extend": {
            "command": "node ./test/env-extend.js",
            "env": {
                "TEST_ENV": "overridden",
                "FOO": "bar"
            }
        }
    },
    "bin": {
        "bnr": "index.js",
        "better-npm-run": "index.js"
    },
    "bugs": {
        "url": "https://github.com/benoror/better-npm-run/issues"
    },
    "contributors": [
        {
            "name": "Benjamin Orozco"
        },
        {
            "name": "Kent C. Dodds"
        }
    ],
    "dependencies": {
        "commander": "^2.9.0",
        "dotenv": "^2.0.0",
        "object-assign": "^4.0.1"
    },
    "description": "Better NPM scripts runner",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "1000ed14b4f77c853de5a5148805f7e74f771cf0",
        "tarball": "https://registry.npmjs.org/better-npm-run/-/better-npm-run-0.0.15.tgz"
    },
    "gitHead": "349b0ad278b5579f6c8de4c46524b8cf9ebf3365",
    "homepage": "https://github.com/benoror/better-npm-run#readme",
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "benoror"
        },
        {
            "name": "galenandrew"
        },
        {
            "name": "gorangajic"
        }
    ],
    "name": "better-npm-run",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/benoror/better-npm-run.git"
    },
    "scripts": {
        "test": "npm run test:env && npm run test:env-extend && npm run test:params && npm run test:command:object && npm run test:command:string && npm run test:silent",
        "test:command:object": "node index.js test:command:object",
        "test:command:string": "node index.js test:command:string",
        "test:env": "node index.js test:env",
        "test:env-extend": "TEST_ENV2=envvar node index.js test:env-extend",
        "test:params": "node index.js test:params --test",
        "test:silent": "node index.js test:command:object -s && node index.js test:command:object --silent"
    },
    "version": "0.0.15"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
