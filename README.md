
# <img src="man/figures/login_hex.png" align="right" width="120" align="right" /> login: User Authentication for Shiny Applications

**Author:** Jason Bryer, Ph.D. <jason@bryer.org>  
**Website:** <https://jbryer.github.io/login/>

<!-- badges: start -->

[![R-CMD-check](https://github.com/jbryer/login/actions/workflows/R-CMD-check.yaml/badge.svg)](https://github.com/jbryer/login/actions/workflows/R-CMD-check.yaml)
[![](https://img.shields.io/badge/devel%20version-0.9.1-blue.svg)](https://github.com/jbryer/login)
[![](https://www.r-pkg.org/badges/version/login)](https://cran.r-project.org/package=login)
[![](https://img.shields.io/badge/doi-10.5281/zenodo.10633322-blue.svg)](https://doi.org/10.5281/zenodo.10633322)

<!-- badges: end -->

This package provides a framework for adding user authentication to
[Shiny](https://shiny.posit.co) applications. This is unique to other
authentication frameworks such as
[ShinyManager](https://datastorm-open.github.io/shinymanager/) and
[shinyauthr](https://github.com/PaulC91/shinyauthr?tab=readme-ov-file)
in that it provides tools for users to create their own accounts and
reset passwords. This is particularly useful for Shiny applications used
to collect data without a pre-existing user management system. User
credentials are stored in any database that supports the
[DBI](https://dbi.r-dbi.org) interface. Passwords are hashed using MD5
in the browser so that unencrypted passwords are never available to the
Shiny server. For an extra layer of security, you can
[salt](https://en.wikipedia.org/wiki/Salt_(cryptography)) the password
before storing it in the database.

Please see the vignette `vignette('login', package = 'login')` for more
details on how to use this package with your Shiny application.
