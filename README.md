RPamisc
================

RPamisc is a package with miscellaneous functions that intend to make using R a little easier.

Vignettes
---------

-   [EDW Discovery](http://htmlpreview.github.io/?https://github.com/rparrish/RPamisc/blob/master/vignettes/EDW_Discovery.html)

SQL functions
-------------

-   `edwSQL()` - primary function for working with SQL databases. Requires a separate .sql file, which is passed to the named resource (alias for a database connection name).
-   `edwQuery()` - similar function that passes a short SQL snippet instead of using a separate file.
-   `edwSave()` - saves a data.frame to an EDW 'Work' database table.
-   `edwTables()`, `edwFetch()`- additional wrapper scripts for RODBC functions that return a list of tables, or table contents. Not as flexible as edwSQL().

Miscelaneous Functions
----------------------

-   `bg_window()` - for a specified CommunityPatientID, gathers all blood glucose results from the 18-24 hour post-op window
-   `bg_window_summary()` - wrapper function for bg\_window for a list of patients.
-   `cat_function()` - The function that started it all, or at least showed how easy it is to get started in writing R packages. This was taken from a tutorial blog post [Writing an R package from scratch](https://hilaryparker.com/2014/04/29/writing-an-r-package-from-scratch/) by Hilary Parker.

Rmarkdown Templates (RStudio)
-----------------------------

-   "First Template" - Used to compose an short data analysis in PDF. Includes a corporate header logo and prompts for information and a structured outline. Requires LaTeX.

Graphics
--------

-   `cusumPlot` - generates a basic CUSUM plot. Code adapted from MDRC.
-   `dotplot.errors` - generates a basic dotplot with confidence bars.
-   `get_CI()` - Determine the confidence intervals for each group based on numerators/denominators

Installation
------------

This package can be installed using devtools with the following:

    devtools::install_github("rparrish/RPamisc")

Contributing
------------

-   Fork it ( <https://github.com/rparrish/RPamisc/fork> )
-   Create your feature branch (git checkout -b my-new-feature)
-   Commit your changes (git commit -am 'Add some feature')
-   Push to the branch (git push origin my-new-feature)
-   Create a new Pull Request
