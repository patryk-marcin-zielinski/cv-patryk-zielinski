# gulp-starter
Simple gulp starter for front-end projects.

## Basic elements

- SASS compiler (please use `.scss` extension or change extension in `gulpfile.js`)
- CSS minify
- JS concat
- JSHint (for ES6)
- Image optimization

## Requirements

- Node.JS &ge; 6.1
- npm &ge; 4.6

## Instruction
1. Fork this repo. Check [GitHub Help](https://help.github.com/articles/fork-a-repo/) if you need help.
2. Install npm packages: `npm install`.
3. Put your files in directories inside `src`.
4. Start using gulp: `gulp`.

## Q&A

### Why uglify() is commented?
During testing [gulpfile.js](gulpfile.js), `gulp-uglify` was throwing an error (check details [here](https://gist.github.com/WojtekWernicki/5bb1a1722ad94ff7c2cbd1f32169188d)). I decided to disable it and `gulp-rename` the line above. JS files will be concated, but won't be minified. Probably this is fault of my computer (Windows 10), so if you want to try does your Node & gulp can minify JS file, just uncomment these two lines and run `gulp`. If you know how to deal with this problem, please make pull request.

### Why `gulp-watch` doesn't trigger on new images?

I don't know why ¯ \\\_(ツ)_/¯ You need to restart gulp, then `gulp-watch` will optimize your photos. If you know how track new photos, please make pull request.

### What does `.keep` file mean?

Nothing. I created these files insides directories, because Git doesn't track empty directories (see this [thread](http://stackoverflow.com/questions/115983/how-can-i-add-an-empty-directory-to-a-git-repository) on Stack Overflow). You can delete them when you put your files inside directories.

## License

[MIT License](LICENSE)