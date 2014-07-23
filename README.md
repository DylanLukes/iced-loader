# coffee-script loader for webpack

## Usage

``` javascript
var exportsOfFile = require("iced!./file.iced");
// => return exports of executed and compiled file.iced

var exportsOfFile2 = require("iced?literate!./file.litcoffee");
// can also compile literate files.
```

[Documentation: Using loaders](http://webpack.github.io/docs/using-loaders.html)

### Recommended configuration

``` javascript
{
	module: {
		loaders: [
			{ test: /\.iced$/, loader: "iced-loader" },
			{ test: /\.(iced\.md|litcoffee)$/, loader: "iced-loader?literate" }
		]
	}
}
```

### Notes

You can also use the `.coffee` extension without any issue. `.iced` is preferred for clarity.

## License

MIT (http://www.opensource.org/licenses/mit-license.php)
