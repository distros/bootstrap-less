# Bootstrap-less

This package contains only the less files of bootstrap.
This should be used when compiling bootstrap from source using less.

This repository is about 220 kb.

This package should be added to your less `paths` settings:

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

The javascript is also included in the `js` directory.

Include all scripts by using the minified file.

    import "bootstrap-less";
    
or include individual scripts.
    
    import "bootstrap-less/js/affix";
    import "bootstrap-less/js/dropdowns";
