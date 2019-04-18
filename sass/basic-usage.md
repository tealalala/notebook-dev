# Basic Usage: Sass

## Materials
* Sass - Ruby Sass (now deprecated)
* Terminal

## Instructions

1. **Editor** - Create Sass file `input.scss` and `output.css`
  * do NOT add CSS to `.css` file, only add to `.scss`

2. **Terminal**

```
# project-directory

sass input.scss input.css

# watch and update SCSS files
sass --watch input.scss:output.css        # used for watching ONE Sass file
sass --watch app/sass:public/stylesheets  # used for watching MULTIPLE Sass files
```

  * `sass input.scss input.css`
    * take note:
      * input scss => `input.scss`
      * output css => `output.css`
    * this command generates: `input.css.map`
  * `--watch` => used during development like a server, need to turn off - compiles Sass
    * Sass watches the `input.scss` file and updates the `output.css`
