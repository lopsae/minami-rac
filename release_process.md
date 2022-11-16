Release process
===============

Set dev version
---------------
Update `package.json`, set `version` to `n.e.w-dev`

Commit message: `bump version to n.e.w-dev`



Develop!
--------
🛠🛠🛠



Create dev package
------------------
With local changes, create a dev package to import to other projects:
```
npm pack
```

In other projects `package.json` point to the locally build package:
```
"minami-rac": "file:../minami-rac/minami-rac-n.e.w-dev.tgz"
```

And update the imported package:
```
npm update minami-rac
```



Start release branch
--------------------
```
git flow release start n.e.w
```



Check changelog update
----------------------
+ update and date n.e.w version



Update versions
---------------
In files:
+ npm `package.json`

Update `package-lock.json` by running:
```
npm install
```

Commit message: `bump version to n.e.w`



Finish tag
----------
```
git flow release finish a.b.c
```



Push tag to origin
------------------
Notice that the tag is prefixed with 'v':
```
git push origin vn.e.w
```



Publish to npm
--------------
```
git checkout main
npm publish
```



Tag in github
-------------
+ In https://github.com/lopsae/minami-rac/releases



Rejoice!
--------
🎉🎉🎉

