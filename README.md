# npmtest-react-markdown

#### basic test coverage for  react-markdown (v2.5.0)  [![npm package](https://img.shields.io/npm/v/npmtest-react-markdown.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-react-markdown) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-react-markdown.svg)](https://travis-ci.org/npmtest/node-npmtest-react-markdown)

#### Renders Markdown as React components

[![NPM](https://nodei.co/npm/react-markdown.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-markdown)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-react-markdown/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-markdown/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-react-markdown/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-react-markdown/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-react-markdown/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-react-markdown/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-react-markdown/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-react-markdown/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-react-markdown/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-markdown/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-react-markdown/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-react-markdown/build/test-report.html](https://npmtest.github.io/node-npmtest-react-markdown/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-react-markdown/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-react-markdown/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-react-markdown/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-markdown/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-markdown/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-markdown/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-react-markdown/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-react-markdown/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "react-markdown",
    "description": "Renders Markdown as React components",
    "version": "2.5.0",
    "keywords": [
        "commonmark",
        "markdown",
        "react",
        "react-component"
    ],
    "main": "src/react-markdown.js",
    "umd": "umd/react-markdown.js",
    "scripts": {
        "build": "NODE_ENV=production webpack && NODE_ENV=production webpack --config webpack.config.demo.js",
        "coverage": "istanbul cover node_modules/.bin/_mocha -- --reporter spec",
        "deploy": "gh-pages-deploy",
        "lint": "eslint .",
        "prepublish": "in-publish && npm run qa || not-in-publish",
        "posttest": "npm run lint",
        "qa": "npm prune && npm test && npm run build",
        "test": "mocha --reporter spec",
        "test-travis": "istanbul cover node_modules/.bin/_mocha --report lcovonly -- --reporter spec",
        "watch": "webpack --config webpack.config.demo.js --watch"
    },
    "repository": {
        "type": "git",
        "url": "git@github.com:rexxars/react-markdown.git"
    },
    "author": "Espen Hovlandsdal <rexxars@gmail.com>",
    "license": "MIT",
    "devDependencies": {
        "@types/react": "^15.0.21",
        "buble-loader": "^0.4.1",
        "chai": "^3.5.0",
        "eslint": "^3.19.0",
        "eslint-config-vaffel": "^5.0.0",
        "eslint-plugin-react": "^6.10.3",
        "gh-pages-deploy": "^0.4.2",
        "istanbul": "^0.4.4",
        "jsdom": "^9.12.0",
        "json-loader": "^0.5.4",
        "lodash.assign": "^4.0.9",
        "mocha": "^3.2.0",
        "mocha-jsdom": "^1.1.0",
        "react": "^15.5.0",
        "react-dom": "^15.5.0",
        "webpack": "^1.13.1"
    },
    "gh-pages-deploy": {
        "noprompt": true,
        "prep": [
            "build"
        ],
        "staticpath": "demo/dist"
    },
    "dependencies": {
        "commonmark": "^0.24.0",
        "commonmark-react-renderer": "^4.2.4",
        "in-publish": "^2.0.0",
        "prop-types": "^15.5.1"
    },
    "types": "./react-markdown.d.ts",
    "peerDependencies": {
        "react": ">=0.13.3"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
