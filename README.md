# Minami-rac

A customized [Minami](https://github.com/Nijikokun/minami) template for [RAC — Ruler and Compass](https://github.com/lopsae/rac).


## Install

```bash
$ npm install --save-dev minami-rac
```


## Usage

Clone repository to your designated `jsdoc` template directory, then:

```bash
$ jsdoc entry-file.js -t path/to/minami-rac
```


### Node.js Dependency

In your projects `package.json` file add a generate script:

```json
"scripts": {
  "generate-docs": "node_modules/.bin/jsdoc --configure .jsdoc.json --verbose"
}
```

In your `.jsdoc.json` file, add a template option.

```json
"opts": {
  "template": "node_modules/minami-rac"
}
```


### License

Minami-RAC is licensed under the [MIT License](https://github.com/lopsae/minami-rac/blob/master/LICENSE).

Minami and JSDoc 3 are licensed under the [Apache2 license](https://github.com/lopsae/minami-rac/blob/master/LICENSE).
