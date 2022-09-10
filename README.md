# Minami-RAC

A customized [Minami](https://github.com/Nijikokun/minami) template for [RAC — Ruler and Compass](https://github.com/lopsae/rac).


## Install

Install into `devDependencies`
```bash
$ npm install --save-dev jsdoc
$ npm install --save-dev minami-rac
```


In your `.jsdoc.json` file, add a template option.
```json
"opts": {
  "template": "node_modules/minami-rac"
}
```


In your projects `package.json` file add a generate script:

```json
"scripts": {
  "generate-docs": "node_modules/.bin/jsdoc --configure .jsdoc.json --verbose"
}
```


### Example `templates` JSDoc Configuration

```json
{
  "templates": {
    "minami" : {
      "homeNavItem": "Minami-RAC",
      "versionNavItem": "1.4.0",
      "showInheritedInNav": false,
      "showMethodsInNav": false,
      "showMembersInNav": false
    },
    "default" : {
      "cleverLinks": false,
      "monospaceLinks": false,
      "includeDate" : false,
      "useLongnameInNav": 3,

    }
}
```

+ `minami.showInheritedInNav` - When set to `true` lists the inherited methods and members in the navigation sidebar of the pages of classes and namespaces; otherwise these elements are hidden
+ `minami.showMethodsInNav` - When set to `true` lists the methods of classes and namespaces in the navigation sidebar of all pages; otherwise these elements are hidden
+ `minami.showMembersInNav` - When set to `true` lists the members of classes and namespaces in the navigation sidebar of all pages; otherwise these elements are hidden
+ `default.useLongnameInNav` - Using an integer will display at most that amount of path elements in the navigation sidebar, any omited path is replaced with ellipsis; `true` displays the full longname, `false` is equivalent to `0` which displays only the last element without any ellipsis


### License

Minami-RAC is licensed under the [MIT License](https://github.com/lopsae/minami-rac/blob/master/LICENSE).

Minami and JSDoc 3 are licensed under the [Apache2 license](https://github.com/lopsae/minami-rac/blob/master/LICENSE).
