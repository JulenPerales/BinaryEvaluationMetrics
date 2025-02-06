# BinaryEvaluationMetrics

![R-CMD-check](https://github.com/JulenPerales/BinaryEvaluationMetrics/actions/workflows/R-CMD-check.yaml/badge.svg)

## Overview
**BinaryEvaluationMetrics** is an R package that provides a collection of methods for evaluating binary classification models. It includes novel metrics developed as part of my dissertation, offering alternatives to traditional accuracy measures.

## Installation
You can install the package directly from GitHub using:

```r
# Install devtools if you haven't already
install.packages("devtools")

# Install BinaryEvaluationMetrics
devtools::install_github("JulenPerales/BinaryEvaluationMetrics")
```

## Features
- **Clayton Skill Score (CSS)**: An alternative to commonly used skill scores for binary classification.
- More metrics to be added...

## Usage
Load the package and use the available functions:

```r
library(BinaryEvaluationMetrics)

# Example usage of Clayton Skill Score
actuals <- c(1, 0, 1, 0, 0, 1, 0, 1, 1, 0)
predictions <- c(0.9, 0.7, 0.8, 0.65, 0.3, 0.2, 0.9, 0.4, 0.1, 0)

css <- clayton_skill_score(predictions, actuals)
print(css)
```

## Contributing
If you’d like to contribute, feel free to fork the repository and submit pull requests!

## License
This package is licensed under the MIT License.
