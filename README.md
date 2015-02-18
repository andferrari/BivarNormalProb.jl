# BivarNormalProb.jl

[![Build Status](https://travis-ci.org/andferrari/BivarNormalProb.jl.svg?branch=master)](https://travis-ci.org/andferrari/BivarNormalProb.jl)

BivarNormalProb.jl contains a julia trascription of matlab files bvn.m and bvnu.m authored by Alan Genz. Original matlab source available from http://www.math.wsu.edu/faculty/genz/software/matlab/bvn.m

Copyright (C) 2013, Alan Genz,  All rights reserved.    

These functions compute bivariate central normal probabilities.


## Installation

```julia
Pkg.clone("https://github.com/andferrari/BivarNormalProb.jl")
```
## Usage

```julia
using BivarNormalProb
bvnu(1.0,2.0,0.5)
```
Computes the probability that `x>1.0` and `y>2.0` where `(x,y)` is normaly distributed with correlation coefficient `0.5`. 

```julia
using BivarNormalProb
bvn(1.0,2.0,3.0,4.0,0.5)
```
Computes the probability that `1.0<x<2.0` and `3.0<y<4.0` where `(x,y)` is normaly distributed with correlation coefficient `0.5`. 