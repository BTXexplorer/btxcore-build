# btxcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install btxcore-build
```

and use and require in your gulp file:

```javascript
var gulp = require('gulp');
var btxcoreTasks = require('btxcore-build');

btxcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var btxcoreTasks = require('btxcore-build');
btxcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/BTXexplorer/btxcore) on the main btxcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/BTXexplorer/btxcore/blob/master/LICENSE).

