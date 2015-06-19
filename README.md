OncoSimul
=========


Code for forward population genetic simulation in asexual populations,
with special focus on cancer progression.  Fitness can be an arbitrary
function of genetic interactions between multiple genes, including
epistasis, order restrictions in mutation accumulation, and order effects.
Simulations so far use continuous-time models and can include driver and
passenger genes.  Also included are functions for simulating random DAGs
of the type found in Oncogenetic Tress, Conjunctive Bayesian Networks, and
other tumor progression models, and for plotting and sampling from single
or multiple realizations of the simulations, including whole-tumor and
single-cell sampling.


The /OncoSimulR directory contains the code for the [BioConductor](http://www.bioconductor.org) package
[OncoSimulR](http://www.bioconductor.org/packages/devel/bioc/html/OncoSimulR.html). The
/miscell-files directory contains additional files so far only related to
the above.


A former version of this code has been used in the paper "Identifying
restrictions in the order of accumulation of mutations during tumor
progression: effects of passengers, evolutionary models, and sampling",
[BMC Bioinformatics, 2015, 16:41](http://www.biomedcentral.com/1471-2105/16/41/abstract).




Installation
============

To use the latest code you first need to [use a development version of
Bioconductor](http://www.bioconductor.org/developers/how-to/useDevel/). Most
of the time, from R you only need to do:


```r
    library(BiocInstaller) 
    useDevel()
```

Then the next will install the development version of the package and its
dependencies, if needed:


```r
    source("http://bioconductor.org/biocLite.R")
    biocLite("OncoSimulR")
```



Licenses and copyright
======================

The OncoSimulR BioConductor package is Copyright 2012-2015 by Ramon
Diaz-Uriarte and under the GPL 3 license.

The file under gitinfo-hooks is Copyright 2011 Brent Longborough, is
part of the
[gitinfo package](https://www.ctan.org/tex-archive/macros/latex/contrib/gitinfo?lang=en),
and is under the LaTeX Project Public License 1.3, which is
[incompatible with the GPL](http://directory.fsf.org/wiki/License:LPPLv1.3a). Note
this file is not part of the OncoSimulR BioConductor package.
