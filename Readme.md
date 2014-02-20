*This repository is a mirror of the [component](http://component.io) module [matthewmueller/grow](http://github.com/matthewmueller/grow). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/matthewmueller-grow`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# grow

  Grow textareas. Will work with any input, including long lines that don't have spaces.

## Example

```html
<textarea id="content"></textarea>
```

```js
grow(content)
```

## Installation

    $ component install matthewmueller/grow

## Implementation

This technique copies the textarea value to a "shadow" div to compute the proper height then updates the textarea.

Loosely based off of https://github.com/jaz303/jquery-grab-bag/blob/master/javascripts/jquery.autogrow-textarea.js

> Note: Use `component/grow` if you only need your textarea to grow from newlines.

## API

### `grow(el, options)`

Initializes a growing textarea. Options include

* `buffer`: sets the amount of buffer space added to the end. Defaults to 20px.

## TODO

* remove jquery dependency (needs a component that gets the computed style)

## License

  MIT
