# Platform.js v1.3.5-9

A platform detection library that works on nearly all JavaScript platforms.

## Disclaimer

Platform.js is for informational purposes only & **not** intended as a substitution for feature detection/inference checks.

## Documentation

* [doc/README.md](https://github.com/bestiejs/platform.js/blob/master/doc/README.md#readme)
* [wiki/Changelog](https://github.com/bestiejs/platform.js/wiki/Changelog)
* [wiki/Roadmap](https://github.com/bestiejs/platform.js/wiki/Roadmap)

## Installation

In a browser:

```html
<script src="platform.js"></script>
```

In an AMD loader:

```js
require(['platform'], function(platform) {/*…*/});
```

Using npm:

```shell
$ npm i --save platform
```

In Node.js:

```js
var platform = require('platform');
```

Usage example:

```js
// on IE10 x86 platform preview running in IE7 compatibility mode on Windows 7 64 bit edition
platform.name; // 'IE'
platform.version; // '10.0'
platform.layout; // 'Trident'
platform.os; // 'Windows Server 2008 R2 / 7 x64'
platform.description; // 'IE 10.0 x86 (platform preview; running in IE 7 mode) on Windows Server 2008 R2 / 7 x64'

// or on an iPad
platform.name; // 'Safari'
platform.version; // '5.1'
platform.product; // 'iPad'
platform.manufacturer; // 'Apple'
platform.layout; // 'WebKit'
platform.os; // 'iOS 5.0'
platform.description; // 'Safari 5.1 on Apple iPad (iOS 5.0)'

// or parsing a given UA string
var info = platform.parse('Mozilla/5.0 (Macintosh; Intel Mac OS X 10.7.2; en; rv:2.0) Gecko/20100101 Firefox/4.0 Opera 11.52');
info.name; // 'Opera'
info.version; // '11.52'
info.layout; // 'Presto'
info.os; // 'Mac OS X 10.7.2'
info.description; // 'Opera 11.52 (identifying as Firefox 4.0) on Mac OS X 10.7.2'
```

## Support

Tested in Chrome 62-63, Chrome Headless 63, Firefox 56-57, IE 11, Edge 15-16, Safari 10-11, Node.js 4-8, & PhantomJS 2.1.1.

## See platform.js in action

[whatsmyua.info](http://www.whatsmyua.info/) shows what platform.js reports for your current user agent/OS/device, or for any arbitrary user agent string.

## BestieJS

Platform.js is part of the BestieJS *“Best in Class”* module collection. This means we promote solid browser/environment support, ES5+ precedents, unit testing, & plenty of documentation.
