# TOML.js [![Build Status](https://travis-ci.org/jcoglan/toml.png)](https://travis-ci.org/jcoglan/toml)

An cross-platform JavaScript TOML parser done properly.


# Supported platforms

* Browsers: see [Testling](http://ci.testling.com/jcoglan/toml)
* Node: see [Travis](https://travis-ci.org/jcoglan/toml)


## Usage

In Node:

```js
var toml = require('toml'),
    fs   = require('fs');

var data = toml.parse(fs.readFileSync('./config.tml').toString());
```

In the browser:

```html
<script type="text/javascript" src="toml-min.js"></script>
<script type="text/javascript">
  var data = TOML.parse('\
               [config]\n\
               foo = "something"\n\
               bar = 42')

  // -> {config: {foo: "something", bar: 42}}
</script>
```


## License

(The MIT license)

Copyright (c) 2013 James Coglan

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

