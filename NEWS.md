# prioritizrdata 0.3.2.2

- Update package manual entry.

# prioritizrdata 0.3.2.1

- Fix aliasing for package manual entry (#14).

# prioritizrdata 0.3.2

- Release candidate for CRAN.
- Update dependency versions.
- Fix README badges.

# prioritizrdata 0.3.1

- Fix documentation to pass CRAN package checks.

# prioritizrdata 0.3.0

- Update the package to use the _sf_ and _terra R_ packages.
- The Salt Spring Island and Tasmania datasets have been updated so
  that they can be imported using the new `get_salt_pu()`,
  `get_salt_features()`, `get_salt_con()`, `get_tas_pu()`, and
  `get_tas_features()` functions.
- The Salt Spring Island dataset now has layer names for the features.
- The Tasmania dataset has updated feature data using NVIS. It also
  contains layer names for the features.
- New Washington dataset as been added. It can be imported using the
  `get_wa_pu()`, `get_wa_features()`, and `get_wa_locked_in()` functions.

# prioritizrdata 0.2.4.2

- Fix tests that fail package checks given only strict dependencies (#8).
- Update citation information in README.
- Remove _rgdal R_ package from Suggests, because it is no longer needed (#10).
- Remove _rgeos R_ package from Suggests, due to pending retirement (#10).

# prioritizrdata 0.2.4.1

- Implement GitHub Actions continuous integration (i.e. update tests
  and README).

# prioritizrdata 0.2.4

- Release candidate for CRAN.

# prioritizrdata 0.2.3.2

- Fix PROJ7 issues with the Tasmania and Salt Spring Island dataset by
  employing a different coordinate reference system (#5).
- Rescale cost values for the Salt Spring Island planning units to avoid
  numerical instability issues when using these data with exact solvers.
- Update Tasmania feature data so that pixels have `NA` values in marine areas.

# prioritizrdata 0.2.3.1

- Assorted documentation improvements (e.g. fixing typos and broken URLs).
- Fix "Non-file package-anchored link(s) in documentation object" warnings
  in R-devel checks.

# prioritizrdata 0.2.3

- Release candidate for CRAN.

# prioritizrdata 0.2.2.1

- Fix spelling of coauthor first name.

# prioritizrdata 0.2.2 (released)

- Release candidate for CRAN.

# prioritizrdata 0.2.1.7

- Remove unneeded Imports.

# prioritizrdata 0.2.1.6

- Update package Description field in DESCRIPTION.

# prioritizrdata 0.2.1.5

- Remove VignetteBuilder from DESCRIPTION since all the vignettes have been
  moved to _prioritizr_.
- Update link to http://www.bcassessment.ca.

# prioritizrdata 0.2.1.4

- Update _prioritizr_ urls with https://prioritizr.net.

# prioritizrdata 0.2.1.3

- The _prioritizr_ package has been removed from Suggests.
- The vignettes have been moved to the _prioritizr_ package.

# prioritizrdata 0.2.1.2

- Assorted documentation improvements.

# prioritizrdata 0.2.1.1

- Depends on R version 3.4.0 (avoids "patchlevel 0" NOTE/WARNING in checks).

# prioritizrdata 0.2.1 (released)

- Release candidate for CRAN.

# prioritizrdata 0.2.0.3

- Fix broken links.
- Tutorials now compatible with _prioritizr_ version 3.0.1.
- Remove Remotes since _prioritizr_ is now on CRAN.

# prioritizrdata 0.2.0.2

- Fix spelling in documentation.
- Update broken links.
- Lint R files.
- Make vignettes compatible with new version of _prioritizr_.
- Add _prioritizr_ to Remotes in DESCRIPTION.

# prioritizrdata 0.2.0.1

- Fix links in README and vignettes.
- Remove log files accidentally committed.
- Fix image size in salt vignette.

# prioritizrdata 0.2.0.0

- Created package website.
- Add _viridis_, _rasterVis_, and _prioritizr_packages to Suggests because they
  are used in the vignettes.
- Remove unused _assertthat_ package from Imports.
- Disable evaluation of code chunk with `library()` calls in _Saltspring.Rmd_
  so that the vignette can be compiled when `lpsymphony`, `Rsymphony` or
  `gurobi` are not installed.
- Package authors now consistent with _prioritizr_ package.
- Simplify vignette workflow. Vignettes can now be compiled by using
  `devtools::build_vignettes()`. Earlier versions needed the vignettes to be
  compiled using the _Makefile_ to copy files around to avoid tangled R code
  causing failures during R CMD CHECK. Although no longer needed, the vignettes
  can still be compiled using the shell command `make vigns` if
  desired.
- The _README.Rmd_ now lives in the top-level directory following standard
  practices. It should now be complied using `rmarkdown::render("README.Rmd")`
  or using the shell command `make readme`. Note that the figures for
  `README.md` can be found in the directory `man/figures`.

# prioritizrdata 0.1.1.0

- Initial package version.
