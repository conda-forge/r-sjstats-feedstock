About r-sjstats
===============

Home: https://github.com/strengejacke/sjstats

Package license: GPL-3

Feedstock license: BSD 3-Clause

Summary: Collection of convenient functions for common statistical computations, which are not directly provided by R's base or stats packages. This package aims at providing, first, shortcuts for statistical measures, which otherwise could only be calculated with additional effort (like standard errors or root mean squared errors). Second, these shortcut functions are generic (if appropriate), and can be applied not only to vectors, but also to other objects as well (e.g., the Coefficient of Variation can be computed for vectors, linear models, or linear mixed models; the r2()-function returns the r-squared value for 'lm', 'glm', 'merMod' or 'lme' objects). The focus of most functions lies on summary statistics or fit measures for regression models, including generalized linear models and mixed effects models. However, some of the functions also deal with other statistical measures, like Cronbach's Alpha, Cramer's V, Phi etc.



Current build status
====================

[![Linux](https://img.shields.io/circleci/project/github/conda-forge/r-sjstats-feedstock/master.svg?label=Linux)](https://circleci.com/gh/conda-forge/r-sjstats-feedstock)
[![OSX](https://img.shields.io/travis/conda-forge/r-sjstats-feedstock/master.svg?label=macOS)](https://travis-ci.org/conda-forge/r-sjstats-feedstock)
[![Windows](https://img.shields.io/appveyor/ci/conda-forge/r-sjstats-feedstock/master.svg?label=Windows)](https://ci.appveyor.com/project/conda-forge/r-sjstats-feedstock/branch/master)

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-r--sjstats-green.svg)](https://anaconda.org/conda-forge/r-sjstats) | [![Conda Downloads](https://img.shields.io/conda/dn/conda-forge/r-sjstats.svg)](https://anaconda.org/conda-forge/r-sjstats) | [![Conda Version](https://img.shields.io/conda/vn/conda-forge/r-sjstats.svg)](https://anaconda.org/conda-forge/r-sjstats) | [![Conda Platforms](https://img.shields.io/conda/pn/conda-forge/r-sjstats.svg)](https://anaconda.org/conda-forge/r-sjstats) |

Installing r-sjstats
====================

Installing `r-sjstats` from the `conda-forge` channel can be achieved by adding `conda-forge` to your channels with:

```
conda config --add channels conda-forge
```

Once the `conda-forge` channel has been enabled, `r-sjstats` can be installed with:

```
conda install r-sjstats
```

It is possible to list all of the versions of `r-sjstats` available on your platform with:

```
conda search r-sjstats --channel conda-forge
```


About conda-forge
=================

conda-forge is a community-led conda channel of installable packages.
In order to provide high-quality builds, the process has been automated into the
conda-forge GitHub organization. The conda-forge organization contains one repository
for each of the installable packages. Such a repository is known as a *feedstock*.

A feedstock is made up of a conda recipe (the instructions on what and how to build
the package) and the necessary configurations for automatic building using freely
available continuous integration services. Thanks to the awesome service provided by
[CircleCI](https://circleci.com/), [AppVeyor](http://www.appveyor.com/)
and [TravisCI](https://travis-ci.org/) it is possible to build and upload installable
packages to the [conda-forge](https://anaconda.org/conda-forge)
[Anaconda-Cloud](http://docs.anaconda.org/) channel for Linux, Windows and OSX respectively.

To manage the continuous integration and simplify feedstock maintenance
[conda-smithy](http://github.com/conda-forge/conda-smithy) has been developed.
Using the ``conda-forge.yml`` within this repository, it is possible to re-render all of
this feedstock's supporting files (e.g. the CI configuration files) with ``conda smithy rerender``.

For more information please check the [conda-forge documentation](https://conda-forge.org/docs/).

Terminology
===========

**feedstock** - the conda recipe (raw material), supporting scripts and CI configuration.

**conda-smithy** - the tool which helps orchestrate the feedstock.
                   Its primary use is in the construction of the CI ``.yml`` files
                   and simplify the management of *many* feedstocks.

**conda-forge** - the place where the feedstock and smithy live and work to
                  produce the finished article (built conda distributions)


Updating r-sjstats-feedstock
============================

If you would like to improve the r-sjstats recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`conda-forge` channel, whereupon the built conda packages will be available for
everybody to install and use from the `conda-forge` channel.
Note that all branches in the conda-forge/r-sjstats-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](http://conda.pydata.org/docs/building/meta-yaml.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](http://conda.pydata.org/docs/building/meta-yaml.html#build-number-and-string)
   back to 0.