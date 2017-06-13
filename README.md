# html-sass-template

Author: WebDesign Master | Modified by Marina Glushakova

OptimizedHTML is all-inclusive, optimized for Google PageSpeed start HTML5 template with Bootstrap (grid only), Gulp, Sass, Browsersync, Autoprefixer, Clean-CSS, Uglify, Imagemin, Vinyl-FTP and Bower (libs path) support. The template contains a .htaccess file with caching rules for web server.

OptimizedHTML Start Template uses the best practices of web development and optimized for Google PageSpeed.

Cross-browser compatibility: IE9+.

The template uses a Sass with Sass syntax and project structure with source code in the directory app/ and production folder dist/, that contains ready project with optimized HTML, CSS, JS and images.

How to use OptimizedHTML

Download optimizedhtml-start-template from GitHub;
Install Node Modules: npm i;
Run the template: gulp.
Gulp tasks:

gulp: run default gulp task (sass, js, watch, browserSync) for web development;
build: build project to dist folder (cleanup, image optimize, removing unnecessary files);
deploy: project deployment on the server from dist folder via FTP;
clearcache: clear all gulp cache.
Rules for working with the starting HTML template

All HTML files should have similar initial content as in app/index.html;
Template Basic Images Start comment in app/index.html - all your custom template basic images (og:image for social networking, favicons for a variety of devices);
Custom Browsers Color Start comment in app/index.html: set the color of the browser head on a variety of devices;
Custom HTML comment in app/index.html - all your custom HTML;
For installing new jQuery library, just run the command "bower i plugin-name" in the terminal. Libraries are automatically placed in the folder app/libs. Bower must be installed in the system (npm i -g bower). Then place all jQuery libraries paths in the 'libs' task (gulpfile.js);
All custom JS located in app/js/common.js;
All Sass vars placed in app/sass/_vars.sass;
All Bootstrap media queries placed in app/sass/_media.sass;
All jQuery libraries CSS styles placed in app/sass/_libs.sass;
Rename ht.access to .htaccess before place it in your web server. This file contain rules for files caching on web server.