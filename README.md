# aidpcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install aidpcore-build
```

and use and require in your gulp file:

```javascript
var gulp = require('gulp');
var aidpcoreTasks = require('aidpcore-build');

aidpcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var aidpcoreTasks = require('aidpcore-build');
aidpcoreTasks('submodule', {skipBrowsers: true});
```

## Contributing

See [CONTRIBUTING.md](https://github.com/underdarkskies/aidpcore) on the main aidpcore repo for information about how to contribute.

## License

Code released under [the MIT license](https://github.com/underdarkskies/aidpcore/blob/master/LICENSE).

