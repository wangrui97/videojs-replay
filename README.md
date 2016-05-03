# videojs-replay

Adds a replay button to video.js player

## Installation

```sh
npm install --save videojs-replay
```

## Usage

To include videojs-replay on your website or web application, use any of the following methods.

### `<script>` Tag

This is the simplest case. Get the script in whatever way you prefer and include the plugin _after_ you include [video.js][videojs], so that the `videojs` global is available.

```html
<script src="//path/to/video.min.js"></script>
<script src="//path/to/videojs-replay.min.js"></script>
<script>
  var player = videojs('my-video');

  player.replay();
</script>
```

### Browserify

When using with Browserify, install videojs-replay via npm and `require` the plugin as you would any other module.

```js
var videojs = require('video.js');

// The actual plugin function is exported by this module, but it is also
// attached to the `Player.prototype`; so, there is no need to assign it
// to a variable.
require('videojs-replay');

var player = videojs('my-video');

player.replay();
```

### RequireJS/AMD

When using with RequireJS (or another AMD library), get the script in whatever way you prefer and `require` the plugin as you normally would:

```js
require(['video.js', 'videojs-replay'], function(videojs) {
  var player = videojs('my-video');

  player.replay();
});
```

## License

MIT or Apache-2.0. Copyright (c) Derk-Jan Hartman


[videojs]: http://videojs.com/
