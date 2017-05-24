
<!-- README.md is generated from README.Rmd. Please edit that file -->
rODE
====

The goal of rODE is to explore R and its S4 classes and their differences with Java and Python while exploring simulations by solving differential equations.

`rODE` is based in the extraordinary physics library for computer simulations OpenSourcePhyisics. Tae a look at <http://opensourcephysics.org>.

The ODE solvers implemented in R so far:

-   Euler
-   Euler-Richardson
-   RK4
-   RK45, Dormand-Prince45
-   Verlet

Installation
------------

You can install rODE from github with:

``` r
# install.packages("devtools")
devtools::install_github("AlfonsoRReyes/rODE")
```

Examples
--------

Example scripts are located under the folder `examples` in the package. These examples make use of a parent class containing a customized rate calculation as well as the step and startup method. The methods that you would commonly find in the base script or parent class are:

-   getRate()
-   getState()
-   initialized(), and
-   the constructor

For instance, the application `KepplerApp.R` needs the class `Kepler` located in the `Kepler.R` script, which is called with `planet <- Kepler(r, v)`, an `ODE` object. The solver for the same application is `RK45` called with `solver <- RK45(planet)`. Since `RK45` is an ODE solver, the script `RK45.R` will be located in the folder `./R` in the package.

``` r
## basic example code
```
