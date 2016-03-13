# videojs-ppc-v4-plugin

Plugin to count pauses and resumes during a video and make an http call to register them

## Table of Contents

<!-- START doctoc -->
<!-- END doctoc -->
## Installation

```sh
npm install --save videojs-ppc-v4-plugin
```

## Usage

To include videojs-ppc-v4-plugin on your website or web application, use any of the following methods.

### `<script>` Tag

This is the simplest case. Get the script in whatever way you prefer and include the plugin _after_ you include [video.js][videojs], so that the `videojs` global is available.

```html
<script src="//path/to/video.min.js"></script>
<script src="//path/to/videojs-ppc-v4-plugin.min.js"></script>
<script>
  var player = videojs('my-video');

  player.ppcV4Plugin();
</script>
```

### Browserify

When using with Browserify, install videojs-ppc-v4-plugin via npm and `require` the plugin as you would any other module.

```js
var videojs = require('video.js');

// The actual plugin function is exported by this module, but it is also
// attached to the `Player.prototype`; so, there is no need to assign it
// to a variable.
require('videojs-ppc-v4-plugin');

var player = videojs('my-video');

player.ppcV4Plugin();
```

### RequireJS/AMD

When using with RequireJS (or another AMD library), get the script in whatever way you prefer and `require` the plugin as you normally would:

```js
require(['video.js', 'videojs-ppc-v4-plugin'], function(videojs) {
  var player = videojs('my-video');

  player.ppcV4Plugin();
});
```

## License

Apache-2.0. Copyright (c) eowynx &lt;maria.antignolo@gmail.com&gt;


[videojs]: http://videojs.com/
