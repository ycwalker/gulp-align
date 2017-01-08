### gulp-align

A gulp plugin which aligns `require` statements in javascript files.

##### Before:

```
var assert = require('chai').assert
var align = require('../index')
var rename = require('gulp-rename')
var fs = require('fs')
var path = require('path')
```

##### After:

```
var assert =  require('chai').assert
var align =   require('../index')
var rename =  require('gulp-rename')
var fs =      require('fs')
var path =    require('path')
```



### Usage

`npm install gulp gulp-align --save-dev`

##### in your `gulpfile.js`

```
gulp.task('align', function () {
    gulp.src('./src/example.js')
        .pipe(align())
        .pipe(gulp.dest('./dist'))
})
```

### License

##### MIT

