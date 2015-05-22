# glob-imagemagick

[![Build Status](https://travis-ci.org/aethermx/glob-imagemagick.svg?branch=master)](https://travis-ci.org/aethermx/glob-imagemagick)
[![Code Climate](https://codeclimate.com/github/aethermx/glob-imagemagick/badges/gpa.svg)](https://codeclimate.com/github/aethermx/glob-imagemagick)

Use a glob pattern to find and resize a set of files with ImageMagick and save them to a new location.

You need to install [ImageMagick](http://www.imagemagick.org/) too.

    # Mac
    brew install imagemagick

    # Ubuntu
    sudo apt-get install imagemagick 

## Install

    npm install glob-imagemagick

## Usage

```js
var resize = require('glob-imagemagick')

var sourceFolder = __dirname + '/images'
var targetFolder = __dirname + '/output'

resize(sourceFolder, ['**/*.png'], targetFolder, '100x100', function(err){
  if ( err ) {
    console.log(err);
  }
})
```

## Running Tests

    npm test

## Legal

[Æther](http://aether.mx/)

hello@aether.mx

[Licensed under the MIT license](http://opensource.org/licenses/mit-license.php)
