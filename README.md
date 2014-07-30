[![Build Status](https://circleci.com/gh/segmentio/load-metadata.png?circle-token=c2b4cfaa8e98f46f9ee24fba69609eb790e500f2)](https://circleci.com/gh/segmentio/load-metadata)

# load-metadata

Load a JSON or YAML metadata file and return it as an object.

## Install

```
npm install load-metadata
```

## Usage

It handles both JSON and YAML and will return a parsed object.

```
var load = require('load-metadata');

load('path/to/metadata.json', function(err, data){
    console.log(data);
});
```

## API

### load(path, callback)

Takes a path to the metadata file. The callback will be called with `fn(err, result)`.

### load.sync(path)

Load a metafile syncronously.