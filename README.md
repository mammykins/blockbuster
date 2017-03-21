
[![Build Status](https://travis-ci.com/mammykins/blockbuster.svg?token=sGXpJU3xjdpxsRrMLhKy&branch=master)](https://travis-ci.com/mammykins/blockbuster)
[![codecov.io](http://codecov.io/github/mammykins/blockbuster/coverage.svg?branch=master)](http://codecov.io/github/mammykins/blockbuster?branch=master)
[![GitHub tag](https://img.shields.io/github/tag/mammykins/blockbuster.svg)]()

# blockbuster

This R package allows you to simulate the deterioration of School buildings through time using a Discrete Time Markov Chain. The data were collected during the Property Data Survey Programme (PDSP) of 2012-2014. Approximately 2.7 million rows of data were collected. This provides the initial state of the School Estate at timestep zero. The deterioration of the School Estate is then modelled by using deterioration rates associated with each Construction Elements-Sub-element-construction-type. Cost of repairs for these building components are estimated. An investment profile for rebuilding and maintaining the School Estate can also be input to mitigate this entropic spiral. Here we provide an anonymised ten percent sample of School buildings or blocks with identifying features removed. During the development period we have some simulated data available to aid code development, real data may be uploaded later or may be available on request.



|Data inputs|Description|
|---|---|
|building condition|Input data for time zero. A sample simulated from the PDS condition data table.|
|transition matrices|Deterioration rates based on estimates of expected lifetime of a building element-sub-element-construction-type.|
|repair costs|Repair costs of building components from condition grades D-B back to A.|
|rebuild costs|Rebuild cost in pounds per metre squared per unit of gross internal floor area to be rebuilt.|

## Installing the package

The package can be installed with the `devtools` package with `devtools::install_github('mammykins/blockbuster')`.

If you cannot use this function (due to firewalls for instance) you can download the package as a `.zip` file from the main repository page, and run `devtools::install_local('path_to_zip_file')`.

## Using the package

### From the terminal


### From an R session

Launch an R session as normal and run the following (again setting the arguments as required):

```
library(blockbuster)
```

Some documentation and vignettes will be added during package development to aid the user.

```

### Project goal

To simulate the deterioration of the School Estate into the future under various maintenance and rebuilding spending policies. This will provide a data driven approach to improving the management of the School Estate saving public money. The models predictions should be evaluated with the next Condition Data Collection due in 2017 and beyond.

### Improvements

Raise an issue.
