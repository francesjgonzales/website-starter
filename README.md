# Website starter file with Gulp, Sass and Browsersync

The purpose of this project is to understand how to automate repetitive tasks for JavaScript-based web development projects.

I use [Gulp](https://gulpjs.com/) as a task runner to minify and concatenate Javascript and CSS files and image optimization. The tool uses API to define tasks and dependencies, and it runs these tasks in a fast and reliable manner. It is built on Node.js and can be installed via npm (Node Package Manager) like any other Node.js module.

\*NOTE: For images, it minifies png, svg, gif and jpg but not Webp file.

[Sample live site](https://comforting-manatee-0abf78.netlify.app/)

## Using MAC terminal to install presets, plugins and dependencies

1. Create a project folder
   `mkdir <project-folder-name>`
2. Switch to your project folder
   `cd <project-folder-name>>`
3. Add JS, SCSS and CSS folders
   `mkdir -p <folder-name-1> <folder-name-2>`
4. Add JS and CSS files in respective nested folders
   `touch <filename.extension>`
5. To go back to root directory
   `cd or cd ..`

## Set up GULP with SASS, SourceMaps, Imagemin & BrowserSync

1. Check if node and npm are installed in global env

   - Node.js - Node.js is an asynchronouse event-driven Javascript runtime
     `node --v`

   - NPM - used to adapt or incporporate packages of code to new and currently building apps
     `npm --v`

   If it's not installed yet:

   - Install latest NPM
     `npm install -g npm`

   - Install [Node.js](https://nodejs.org/en/download)

2. Set up [SASS](https://sass-lang.com/) in your project folder

   - Install Node-sass to compile `.scss` and `.css`
     `npm install node-sass --save-dev`

   - Add this in your package.json
     `"compile-sass": "node-sass sass/main.scss css/style.css`

3. Install Gulp and its plugins

   1. Check if Gulp is installed globally

      - To check Gulp version
        `gulp --version`

      - If its not install, install the gulp command utility
        `npm install --global gulp-cli`

   2. Create a project directory and switch to it

   3. Create a package.json file in your project directory
      `npm init`

   4. Install Gulp in your project directory

      - `npm install --save-dev gulp`

      - Verify your gulp version
        `gulp --version`

   5. Install the following [Gulp plugins](https://gulpjs.com/plugins) for website starter boilerplate

      - _autoprefixer_ - Prefix CSS
      - _cssnano_ - Minify CSS with cssnano
      - _concat_ - Concatenates files
      - _postcss_ - to pipe CSS through several plugins, but parse CSS only once
      - _replace_ - A string replace plugin for gulp
      - _sourcemaps_ - Sourcemaps solve the debugging problem by providing a mapping between the original source code and the compressed version
      - [_terser_](https://terser.org/) - compressor toolkit for ES6+. It removes comments, makes variable names smaller, and removes whitespace
      - [_browser-sync_](https://browsersync.io/) - live-testing browser that cuts out repetitive manual testing tasks from replication to click mirroring
      - [_imagemin_](https://www.npmjs.com/package/gulp-imagemin)
        - [gifsicle](https://www.npmjs.com/package/imagemin-gifsicle) — Compress GIF images, lossless. Reduce the number of distinct colors in each output GIF to num or less. Num must be between 2 and 256. This helps to minify the filesize but quality will be poor
        - mozjpeg — Compress JPEG images, lossy
        - optipng — Compress PNG images, lossless
        - svgo — Compress SVG images, lossless

      **Run this code to install the plugins**
      `npm install --save-dev gulp-autoprefixer gulp-cssnano gulp-concat postcss gulp-postcss gulp-replace sass gulp-sass gulp-sourcemaps gulp-terser gulp-browser-sync gulp-imagemin gulp-webp`

## Set up testing environment using JEST

1.

# To implement

- _webp_ - Convert images to WebP. I enncounter error: ERR_REQUIRE_ESM when I install gulp-webp plugin. Downgrading gulp created another error called ReferenceError: primordials is not defined. Using webp image in the starter file still works but have yet to test it properly.

# Resources:

- [Browser-sync](https://youtu.be/q0E1hbcj-NI)
- [Gulp 4 Crash Course for Beginners](https://youtu.be/-lG0kDeuSJk)
- [Minify webp images](https://www.youtube.com/watch?v=ubHwScDfRQA&t=958s)
- [How to resolve ERR_REQUIRE_ESM](https://stackoverflow.com/questions/69862766/getting-error-err-require-esm-while-running-gulp-command)

# Credits

Thanks to the following:

- [Coding in Public](https://www.youtube.com/@CodinginPublic)
- [Coder Coder](https://www.youtube.com/@TheCoderCoder)
