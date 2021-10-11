# Survival-of-packages-on-CRAN
## Background
There are a lot of R packages on CRAN, with the number growing exponentially over time. However, not all the packages stay there: they may be removed from the live version of CRAN by the author’s request or because they don’t work with the current version of R. All current and past packages are stored in the
CRAN archive.

In recent years, many more people have been writing packages, and packages have tended to have more dependencies on other packages. This might be expected to lead to packages that don’t last as long.

## The file alldates.rda contains a single data frame all_dates, with variables listed as follows:

**pkg**: the name of the package

**cran_date**: the date the current version was put on CRAN

**first**: the oldest date when a version was put into archive

**latest**: the most recent date when a version was put into archive

**Note**: The dates are offsets from **1970/1/1**

## The file snapshots.rda contains two data frames:

a: the result of `available.packages()`, a matrix listing all available CRAN packages on 2020-6-2.

b: the result of `available.packages()` as it would have been on 2015-6-2, via the Microsoft CRAN Time
Machine.

## Our Tasks are:
1. Describe how the longevity of CRAN packages has changed over time

2. Describe how version number, dependencies, and license relate to the probability of a **2015** package surviving to **2020** (as a binary outcome)

3. Describe how dependencies, and license relate to the subsequent survival time of a package on CRAN in **2015**
