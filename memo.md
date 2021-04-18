# process to deploy a js project

1. install gh-pages in dev dependencies

```
npm install gh-pages --save-dev
```

2. inside ``package.json`` add (i.e. on top for my starlord-player project) :

```
"homepage": "http://andonary.github.io/starlord-player",
```

3. inside ``package.json`` add in ``scripts`` :

```
"scripts": {
    ...
    "predeploy": "npm run build",
    "deploy": "gh-pages -d build"
    }
```

4. run predeploy and deploy script :

```
npm run predeploy
npm run deploy
```

5. think to commit/tag/push or usual stuff, then it's finished
