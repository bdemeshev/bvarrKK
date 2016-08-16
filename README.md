bvarr
=====

The package `bvarrKK` may be useful for estimating bayesian VAR models.

It contains a translation to R of the matlab code by
[Gary Koops and Dimitris Korobilis](http://personal.strath.ac.uk/gary.koop/bayes_matlab_code_by_koop_and_korobilis.html) with minor improvements.

You may install the package usinge the commands:
```R
install.packages("devtools")
devtools::install_github("bdemeshev/bvarrKK")
```

Replication of KK code:
```R
library("bvarr")
data(Yraw)
model <- bvar(Yraw,prior = "independent")
bvar.imp.plot(model)
bvar.summary(model)
```

This code is not developed anymore. You are free to start...


You may also wish look at [BMR](http://bayes.squarespace.com/bmr/), [MSBVAR](http://cran.r-project.org/web/packages/MSBVAR/), [bvarsv](https://cran.r-project.org/web/packages/bvarsv/index.html) packages. 


[![Travis-CI Build Status](https://travis-ci.org/bdemeshev/bvarrKK.svg?branch=master)](https://travis-ci.org/bdemeshev/bvarrKK)


