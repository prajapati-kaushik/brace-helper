brace-helper
============

Brace helper will look for HTML5 elements with a given classname (`.ace-editor` by default) and turns them into an [ace editor](https://ace.c9.io/) using [brace](https://github.com/thlorenz/brace)

## Example

package.json
```json
{
  "dependencies": {
    "brace": "^0.11.1",
    "brace-helper": "^0.1.0",
  }
}
```

app.js:
```javascript
require('brace'); // require brace for main functionality
require('brace-helper'); // auto initialize ace editors

// require any modes or themes you'd like to use in your app
require('brace/mode/javascript');
require('brace/mode/css');
require('brace/mode/yaml');
require('brace/theme/monokai');
```

example.html:
```html
<textarea class="ace-editor" data-mode="css" data-lines="50"></textarea>
```

This textarea will now be automatically converted into an ace editor with css highlighting.


## Inspiration

This library was inspired by [ace-helper](https://github.com/h-wang/ace-helper), but can be used in a webpack / browserify / webpack-encore environment, and does not require jQuery.

## License

MIT. Please refer to the [license file](LICENSE) for details.

## Brought to you by the LinkORB Engineering team

<img src="http://www.linkorb.com/d/meta/tier1/images/linkorbengineering-logo.png" width="200px" /><br />
Check out our other projects at [linkorb.com/engineering](http://www.linkorb.com/engineering).

Btw, we're hiring!