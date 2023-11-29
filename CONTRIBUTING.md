**Hint** is written in [SASS](http://sass-lang.com/).

# Setup

1. [Fork **Hint.css**](https://help.github.com/articles/fork-a-repo) and clone it on your system.
2. Create a new branch out off `master` for your fix/feature. `git checkout new-feature master`

# Building

**Hint.css** uses [Grunt](http://gruntjs.com/) for the build process which you need to have installed on your system.

Also there are four additional Grunt tasks required to build the library:

1. [grunt-contrib-cssmin](https://npmjs.org/package/grunt-contrib-cssmin)

2. [grunt-sass](https://www.npmjs.com/package/grunt-sass)

3. [grunt-contrib-concat](https://www.npmjs.com/package/grunt-contrib-concat)

4. [grunt-contrib-watch](https://www.npmjs.com/package/grunt-contrib-watch)

To install all the dependencies, run `npm install`.

Once you have the dependencies installed, run `npm run dev` from the project directory. This will start watching all the files in `src/` and run the default grunt task which compiles the SCSS files into `hint.css` file. You can then test your changes in `demo.html`.

Though this should be sufficient for building the library for testing, in case you want to build the minified version as well you can run the `grunt deploy` command instead.

# Things to remember

- Do not fix multiple issues in a single commit. Keep them one thing per commit so that they can be picked easily incase only few commits require to be merged.

- For every new modifier (example `hint--success`, `hint--top`) added, make a separate file unless it fits into a current modifier file.

- Before submitting a patch, rebase your branch on upstream `master` to make life easier for the merger.

- **DO NOT** add the library builds (`hint.css` & `hint.min.css`) in your commits.

# Stay in touch

Best place to get in touch regarding this library is the [issues board on Github](https://github.com/chinchang/hint.css/issues).
