NEWS
====

Versioning
----------

Releases will be numbered with the following semantic versioning format:

&lt;major&gt;.&lt;minor&gt;.&lt;patch&gt;

And constructed with the following guidelines:

* Breaking backward compatibility bumps the major (and resets the minor 
  and patch)

* New additions without breaking backward compatibility bumps the minor 
  (and resets the patch)

* Bug fixes and misc changes bumps the patch



**CHANGES** IN <a href="https://github.com/trinker/pax" target="_blank">pax</a> VERSION 0.2.0 -
----------------------------------------------------------------

**BUG FIXES**

**NEW FEATURES**

* `arg_rep` added for easy passing through of arguments from a main function to 
  a helper function.
  
* `arg_assign` added for easy assignment of arguments (especially when there are 
  defaults) for testing/code writing purposes.
  
**MINOR FEATURES**

**IMPROVEMENTS**

**CHANGES**



**CHANGES** IN <a href="https://github.com/trinker/pax" target="_blank">pax</a> VERSION 0.1.0
----------------------------------------------------------------

First stable release.

**BUG FIXES**

* `new_data` did not save a usable data file.  This have been corrected 
  (2015-05-27).

**NEW FEATURES**

* `new_data` added to quickly add data sets and accompanying **roxygen2** style 
  template to the package description *.R* file.

* `new_r` adds support for print ad plot methods.

**MINOR FEATURES**

**IMPROVEMENTS**

* A *package-package.R* file is added to the *R* directory that describes the 
  package in the documentation.  This is also where **roxygen2** style 
  formatting is added to document data sets.

* `pax` now used **rmarkdown** to render the `README.md` file.

**CHANGES**

**CHANGES** IN <a href="https://github.com/trinker/pax" target="_blank">pax</a> VERSION 0.0.3
----------------------------------------------------------------

**BUG FIXES**

* `pax::pax`  Missed a package name insertion in the README.Rmd file for the 
  Travis-CI link.

* `pax::pax` created a **travis.yml** file, missing the leading dot.  Replaced 
  with **.travis.yml**.

* `pax::pax` had incorrect link to coverage badge as package and GitHub name were
  reversed.

**NEW FEATURES**

* `new_r` added to quickly produce a **roxygen2** style .R template file from a 
  `function` (output file will include the function) or a character string.

* `new_test` added to quickly produce a **testthat** style test .R template file 
   from a `function` (output file will include the function) or a character string.

* `new_r_test` added to combine the functionality of `new_r` and `new_test` into 
  one call.

* `pax_options` added to generate a script template of blank **pax** options 
  that can be added to *.Rprofile*.

* `new_vignette` added to quickly add **rmarkdown** style vignette tempaltes.


**MINOR FEATURES**

* **staticdocs** website is up and running: http://trinker.github.io/pax/  
  Improvements to come.

* `pax::pax`'s `sample` argument is now set to `getOption("samples")`.  The 
  argument can now be set via .Rprofile.

**IMPROVEMENTS**

* The **README.Rmd** uses *.svg* badges rather than *.png* badges.


**CHANGES** IN <a href="https://github.com/trinker/pax" target="_blank">pax</a> VERSION 0.0.2
----------------------------------------------------------------

`pax` is considered ready for use.


**NEW FEATURES**

* `ploc` added to allow the user to (1) set a package directory location in the 
  .Rprofile and (2) supply a package name to create a file path.  Useful with
  `pax` function to supply just a package name and the package is placed in a 
  standard location.


**CHANGES** IN <a href="https://github.com/trinker/pax" target="_blank">pax</a> VERSION 0.0.1
----------------------------------------------------------------

* The first GitHub installation of the <a href="https://github.com/trinker/pax" target="_blank">pax</a> package

* Package designed to provide a package templating system that assumes the use 
  of **testthat**, Travis-CI, RStudio, **devtools**, and **covr** (coveralls).