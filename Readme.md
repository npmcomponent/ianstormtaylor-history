*This repository is a mirror of the [component](http://component.io) module [ianstormtaylor/history](http://github.com/ianstormtaylor/history). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/ianstormtaylor-history`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# history

  A nicer wrapper around the browser's History API. Push, replace, back, forward, etc.

## Installation

    $ component install ianstormtaylor/history

## Example

```js
var history = require('history');

history.push('/one');
history.push('/two');
history.back();
history.path(); // "/one"
```

## API

### .path()
  Get the current path. (`window.location.pathname`)

### .state()
  Get the current state. (`window.history.state`)

### .push(path, [state])
  Push the `path` onto the history stack, with an optional `state` object.

### .replace(path, [state])
  Replace the current path with a new `path`, and optional `state` object.

### .back(steps)
  Move backward an optional number of `steps`, defaults to `1`. Aliased to `backward()` for consistency.

### .forward(steps)
  Move forward an optional number of `steps`, defaults to `1`.

## License

  MIT
