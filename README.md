# npm-check-engines

Check that your dependencies support your supported engines.

```
npm install -g npm-check-engines
```

## Wait, what?

You specify the supported engines in your [package.json](https://docs.npmjs.com/files/package.json#engines):

```
"engines": {
  "node": ">= 4.0"
}
```

If any of your dependencies do not support any version `>= 4.0` (4.0, 4.1, 4.2, 5.0 and so on),
this script will tell you. It works by fetching a list of Node releases and then
iterating over all dependencies.
