# grunt-contrib-requirejs [![Build Status](https://secure.travis-ci.org/gruntjs/grunt-contrib-requirejs.png?branch=master)](http://travis-ci.org/gruntjs/grunt-contrib-requirejs)

> Optimize RequireJS projects using r.js.


## Getting Started
If you haven't used [grunt][] before, be sure to check out the [Getting Started][] guide, as it explains how to create a [gruntfile][Getting Started] as well as install and use grunt plugins. Once you're familiar with that process, install this plugin with this command:

```shell
npm install grunt-contrib-requirejs --save-dev
```

[grunt]: http://gruntjs.com/
[Getting Started]: https://github.com/gruntjs/grunt/blob/devel/docs/getting_started.md


## Requirejs task
_Run this task with the `grunt requirejs` command._

### Overview

In your project's Gruntfile, add a section named `requirejs` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  requirejs: {
    options: {
      // Task-specific options go here.
    },
    your_target: {
      // Target-specific file lists and/or options go here.
    },
  },
})
```

Options are passed to the [RequireJS Optimizer](http://requirejs.org/docs/optimization.html).
### Options

For a full list of possible options, [see the r.js example build file](https://github.com/jrburke/r.js/blob/master/build/example.build.js).
### Examples

```js
requirejs: {
  compile: {
    options: {
      baseUrl: "path/to/base",
      mainConfigFile: "path/to/config.js",
      out: "path/to/optimized.js"
    }
  }
}
```

## Release History

 * 2012-10-11   v0.3.3   Rename grunt-contrib-lib dep to grunt-lib-contrib.
 * 2012-10-08   v0.3.1   Bump to RequireJS 2.1.x. Run optimizer async.
 * 2012-09-22   v0.3.0   Options no longer accepted from global config key.
 * 2012-09-09   v0.2.0   Refactored from grunt-contrib into individual repo.

---

Task submitted by [Tyler Kellen](http://goingslowly.com/)

*This file was generated on Mon Nov 19 2012 16:03:32.*
