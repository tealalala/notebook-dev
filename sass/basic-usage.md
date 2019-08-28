# Basic Usage: Sass

## Materials
* Sass (Dart-Sass)
* Terminal

## Instructions

1. **Editor** - Create Sass file `input.scss` and `output.css`
  * do NOT add CSS to `.css` file, only add to `.scss`

2. **Terminal**

```
# project-directory

# manual compile scss => css
sass input.scss:input.css

# dynamic compile scss => css: watch and update SCSS files
sass --watch input.scss:output.css        # used for watching ONE Sass file
sass --watch app/sass:public/stylesheets  # used for watching MULTIPLE Sass files

# style conversion scss => css: expand, compact, or compress
sass --watch --style expand input.scss:output.css     # expand nested => expand
sass --watch --style compact input.scss:output.css    # compact => compiles css into one-liner
sass --watch --style compressed input.scss:output.css # compress => compiles removes all spaces and line breaks (think of minified css)
```

  * `sass input.scss input.css`
    * take note:
      * input scss => `input.scss`
      * output css => `output.css`
    * this command generates: `input.css.map`
  * `--watch` => used during development like a server, need to turn off - compiles Sass
    * Sass watches the `input.scss` file and updates the `output.css`
