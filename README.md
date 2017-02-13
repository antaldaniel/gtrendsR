
## gtrendsR [![Travis-CI Build Status](https://api.travis-ci.org/PMassicotte/gtrendsR.svg?branch=master)](https://travis-ci.org/PMassicotte/gtrendsR) [![AppVeyor Build Status](https://ci.appveyor.com/api/projects/status/github/PMassicotte/gtrendsR?branch=master&svg=true)](https://ci.appveyor.com/project/PMassicotte/gtrendsR) [![Package-License](https://img.shields.io/badge/license-GPL%20%28%3E=%202%29-brightgreen.svg?style=flat)](http://www.gnu.org/licenses/gpl-2.0.html) [![CRAN](http://www.r-pkg.org/badges/version/gtrendsR)](https://cran.r-project.org/package=gtrendsR) [![Downloads](http://cranlogs.r-pkg.org/badges/gtrendsR?color=brightgreen)](http://www.r-pkg.org/pkg/gtrendsR)

`gtrendsR` provides an interface for retrieving and displaying Google Trends
information.

Trends (number of hits) over time as well as geographic representation of the results can be displayed.

### Example

In this simple example, trends for keywords `nhl`, `nba` are retrieved for Canada and USA and then plotted from R.

``` {.r}
library(gtrendsR)

res <- gtrends(c("nhl", "nba"), geo = c("CA", "US"))
plot(res)
```

### Installation

Since release 1.3.0, the package is on [CRAN](https://cran.r-project.org) and
can be installed via

``` {.r}
install.packages("gtrendsR")
```

Pre-release versions can be install directly from this repository via

``` {.r}
if (!require("devtools")) install.packages("devtools")
devtools::install_github("PMassicotte/gtrendsR")
```

### Authors

Philippe Massicotte and Dirk Eddelbuettel

### License

GPL (>= 2)

