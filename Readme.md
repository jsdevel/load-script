# jsdevel-load-script

Dynamic script loading.

## Note
This is fork of `eldargab/load-script`.  That fork has not bee touched in a year
and I needed some features not available there.  If these changes get merged back into
upstream, then I will unpublish this module.  Here is where `jsdevel-load-script` differs:

* The module now accepts 3 params `url, [opts,] [cb]`
* Opts can take `attrs` or `text`.
* The script node is passes as the second argument to the callback.

## Installation

via component

```
$ component install jsdevel/jsdevel-load-script
```

via npm

```
$ npm install jsdevel-load-script
```

## API

```javascript
var load = require('jsdevel-load-script')

load('foo.js', function (err) {
  if (err) {
    // print useful message
  }
  else {
    // use script
    // note that in IE8 and below loading error wouldn't be reported
  }
})
```

## License

MIT
