[![Build Status](https://travis-ci.org/Yapapaya/_ya.svg?branch=master)](https://travis-ci.org/Yapapaya/_ya)

# _ya

`_ya` is a starter (bolierplate) theme for the [`wp-get-go` framework](https://github.com/yapapaya/wp-get-go), based on [`_s` by Automattic](https://github.com/Automattic/_s).

If you wish to use this for development outisde `wp-get-go`, please consider using `_s` instead.

## _ya vs _s

 * The `sass` directory is restructured to work with `wp-get-go`
   * The `variables-site` sub-directory is renamed to `variables`
   * All sub-directories have been reorganised so as to have an `.scss` file with the same name as the directory. This file contains all the `@import` statements for other partial `.scss` files in the sub-directory.
   * For example, `variables` contains a file `_variables.scss` that contains `@import` statements for the other two files in this directory `_typography.scss` and `_colors.scss`.
   * Similarly, `elements` contains a file `_elements.scss` but unlike `_s`, it doesn't contain style definitions. They are moved into `_misc.scss`. The `_elements.scss` instead contains only `@import` statements for `_misc.scss`, `_lists.scss`, `_images.scss` and `_tables.scss`.
 * The `layouts` directory is removed. Layouts are expected to be done by a grid or layout component.
 * The informational files, viz., `README.md` (this file), `readme.txt`, `CONTRIBUTING.md` are rewritten.
 * The `style.scss` is restructured and rewritten to work with `wp-get-go` with some extra help information. 
