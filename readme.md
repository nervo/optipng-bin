# node-optipng [![Build Status](https://secure.travis-ci.org/yeoman/node-optipng.png?branch=master)](http://travis-ci.org/yeoman/node-optipng)

[OptiPNG](http://optipng.sourceforge.net) 0.7.4 Node.js wrapper that makes it seamlessly available as a local dependency on OS X, Linux and Windows.


## Example usage

```js
var execFile = require('child_process').execFile;
var optipngPath = require('optipng').path;

execFile(optipngPath, ['-v'], function(err, stdout, stderr) {
	console.log('OptiPNG version:', stdout.match(/\d\.\d.\d/)[0]);
});
```

You can also run it directly from `./node_modules/.bin/optipng`


## License

Everything excluding the binaries licensed under the [BSD license](http://opensource.org/licenses/bsd-license.php)

OptiPNG licensed under the [zlib license](http://optipng.sourceforge.net/license.txt)