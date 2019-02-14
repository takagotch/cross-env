### cross-env
---
https://github.com/kentcdodds/cross-env

```json
{
  "scripts": {
    "greet": "cross-env-shell GREETING=Hi NAME=Joe \"echo $GREETING && echo $NAME\""
  }
}

{
  "scripts": {
    "build": "cross-env NODE_ENV=production webpack --config build/webpack.config.js"
  }
}

{
  "scripts": {
    "parentScript": "cross-env GREET=\"Joe\" npm run childScript",
    "childScript": "cross-env-shell \"echo Hello $GREET\""
  }
}

{
  "scripts": {
    "test": "cross-env TS_NODE_COMPILER_OPTIONS={\\\"module\\\":\\\":\\\"commonjs\\\"} node some_file.test.js"
  }
}

{
  "scripts": {
    "greet": "cross-env-shell GREETING=Hi NAME=Joe \"echo $GREETING && $NAME\""
  }
}
```


```
npm install --save-dev cross-env
webpack --config build/webpack.config.js
```

```
```


