# Website starter file with Gulp, Sass and Browsersync

## Use your MAC terminal to install packages, plugins and dependencies

1. `mkdir <project-folder-name>` - to create a project folder
2. `cd <project-folder-name>>` to switch to your project folder
3. `mkdir -p <folder-name-1> <folder-name-2>` to create multiple folders
4. `touch <filename.extension>` to create a file inside a folder
5. `cd or cd ..` to go back to root folder

## Set up GULP with SASS and BrowserSync

1. Check if node and npm are installed in global env
   `node --v` for node.js (Node.js is an asynchronouse event-driven Javascript runtime)
   `npm --v` for npm (npm is used to adapt or incporporate packages of code to new and currently building apps)

   If it's not installed yet:

   - Install latest npm
     `npm install -g npm`

   - Install (node)[https://nodejs.org/en/download]

2. Install SASS in your project folder
   `npm install -g sass`

   - [How to install SASSS in local project] (https://dev.to/rembertdesigns/setting-up-sass-on-your-local-server-ko1)

3. Install Gulp and plugins

   1. Check if Gulp is installed globally
      `gulp --version`

      - If its not install, install the gulp command utility
        `npm install --global gulp-cli`

   2. Create a project directory and navigate into it
   3. Create a package.json file in your project directory
      `npm init`
   4. Install Gulp in your project directory
      `npm install --save-dev gulp`
      - Verify your gulp version
        `gulp --version`
   5. Install (Gulp plugins)[https://gulpjs.com/plugins] for website starter boilerplate

      - _autoprefixer_ - Prefix CSS
      - _cssnano_ - Minify CSS with cssnano
      - _concat_ - Concatenates files
      - _postcss_ - to pipe CSS through several plugins, but parse CSS only once
      - _replace_ - A string replace plugin for gulp
      - _sourcemaps_ - Sourcemaps solve the debugging problem by providing a mapping between the original source code and the compressed version
      - (_terser_)[https://terser.org/] - compressor toolkit for ES6+. It removes comments, makes variable names smaller, and removes whitespace
      - (_browser-sync_)[https://browsersync.io/] - live-testing browser that cuts out repetitive manual testing tasks from replication to click mirroring
      - _imagemin_ - Minify PNG, JPEG, GIF and SVG images

      **Run this code to install the plugins**
      `npm install --save-dev gulp-autoprefixer gulp-cssnano gulp-concat postcss gulp-postcss gulp-replace sass gulp-sass gulp-sourcemaps gulp-terser gulp-browser-sync gulp-imagemin gulp-webp`

# To implement

- _webp_ - Convert images to WebP. Encounter error: ERR_REQUIRE_ESM

# Resources:

- (Browser-sync)[https://youtu.be/q0E1hbcj-NI]
- (Gulp 4 Crash Course for Beginners)[https://youtu.be/-lG0kDeuSJk]
- (Minify webp images)[https://www.youtube.com/watch?v=ubHwScDfRQA&t=958s]
- (How to resolve ERR_REQUIRE_ESM)[https://stackoverflow.com/questions/69862766/getting-error-err-require-esm-while-running-gulp-command]

# Credits

Thanks to the following:

- (Coding in Public)[https://www.youtube.com/@CodinginPublic]
- (Coder Coder)[https://www.youtube.com/@TheCoderCoder]
