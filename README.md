# Bootstrap-less

This package contains only the less files of bootstrap.
This should be used when compiling bootstrap from source using less.

This repository is about 607 kb.

## Installation

    npm install bootstrap-less

This package should be added to your less `paths` settings.

    gulp.pipe(less({
        paths: [
            '.',
            './node_modules/bootstrap-less'
        ]
    }))

Then bootstrap can be included in any less file.

    @import "bootstrap/index";
    
Or individual files can be imported instead of the index.

    @import "bootstrap/grid";
    @import "bootstrap/dropdowns";
    
## Javascript

The javascript is included in the `js` directory.

when using jspm the package can be installed from npm.

    jspm install bootstrap-less

Include all scripts by using the compiled version file.

    import "bootstrap-less";
    
or include individual scripts if only some scripts are needed.
    
    import "bootstrap-less/js/affix";
    import "bootstrap-less/js/dropdowns";
