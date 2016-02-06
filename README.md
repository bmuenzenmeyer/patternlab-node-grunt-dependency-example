# Pattern Lab Node Grunt Dependency Example

Making Pattern Lab Node a dependency allows you to host your source and public patterns and assets outside of the module, making upgrades easier.

This repository is a reference example of a fully configured parent project that uses [Pattern Lab Node](https://github.com/pattern-lab/patternlab-node) as a dependency. `node_modules` are not included out of sanity, but running `npm install` from this cloned repository will show that it is indeed a dependency along with everything else.

The example `patternlab-config.json` contains a paths object that defined absolute paths (C:/src/plnd/) to the installation of this example. **You will have to change this if you expect anything to run here.**

``` json
"paths" : {
  "source" : {
    "root": "C:/src/plnd/source/",
    "patterns" : "C:/src/plnd/source/_patterns/",
    "data" : "C:/src/plnd/source/_data/",
    "styleguide" : "C:/src/plnd/node_modules/patternlab-node/core/styleguide/",
    "patternlabFiles" : "C:/src/plnd/source/_patternlab-files/",
    "js" : "C:/src/plnd/source/js",
    "images" : "C:/src/plnd/source/images",
    "fonts" : "C:/src/plnd/source/fonts",
    "css" : "C:/src/plnd/source/css/"
  },
  "public" : {
    "root" : "C:/src/plnd/public/",
    "patterns" : "C:/src/plnd/public/patterns/",
    "data" : "C:/src/plnd/public/data/",
    "styleguide" : "C:/src/plnd/public/styleguide/",
    "js" : "C:/src/plnd/public/js",
    "images" : "C:/src/plnd/public/images",
    "fonts" : "C:/src/plnd/public/fonts",
    "css" : "C:/src/plnd/public/css"
  }
},
```

Documentation that attained this state can be found [here](https://github.com/pattern-lab/patternlab-node/wiki/Running-Pattern-Lab-Node-as-an-NPM-Dependency).
