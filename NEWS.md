# splitTools 0.3.2

This is documentation and maintenance update only with the following changes:

- Updated documentation to clarify that `create_folds()` creates in-sample indices by default. If out-of-sample indices are to be generated, set `invert = TRUE`.
- Got rid of a CRAN check notes about LazyData.
- Changed to better way of updating/generating the package.

# splitTools 0.3.1

## New Functionality

- `create_folds` and `partition` have received a `shuffle` option to shuffle rows within folds/partitions. The default is FALSE.

# splitTools 0.3.0

## Breaking change for tiny data sets

- `create_folds` and `partition` cannot return empty folds/partitions anymore. This impacts only extremely small data sets.

## Other

- Unit tests have been added.

# splitTools 0.2.1

## New Functionality

- `create_timefolds` now allows also moving windows training data, not just extending windows data.

## Other

Reduced minimally required R version from 3.5 to 3.1.

# splitTools 0.2.0

## New Functionality

- Added `type = "blocked"` to `create_folds` and `partition` to allow for blocked splitting.

- Added function `create_timefolds` for cross-validation of time series data.

## Other

Added vignette

# splitTools 0.1.0

This is the initial CRAN release.
