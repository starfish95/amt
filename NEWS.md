# amt 0.0.7

## new features
- Added a dplyr count method for track, steps, random_steps and random_points
- Added a AIC method for `fit_(i)ssf`.
- Added for KDE: pi and lscv for bandwidth estimation


## major changes
- `hr_locoh_k` id deprecated and will be part of `hr_locoh`. Specifically `type = "k"`. 
- All home range methods now return `sf` objects.



# amt 0.0.6.0
## major changes
- random_points with kde home ranges now work with different home range levels. 
- random_steps now uses `units` to be explicit about the turning angle.
- `bbox` is also available for steps and can return objects of `sf`.



# amt 0.0.5.0
## major changes
- `random_steps` gained a new distribution for random steps (exponential).
- bug fix in `random_steps`
- new function `extract_covariates_along`, extracts covariates along a random step.
- `steps` gains a new argument: `keep_cols` in order to keep columns from point when creating steps.
- `simulate_tud`: a convenience wrapper arround `simulate_ud` to simulate transition UDs.
# amt 0.0.4.0
## major changes
- Added an alias to `mk_track` called `make_track`.
- `mk_track` gained a new argument `all_cols` that allows to carry over all columns to track.
- `mk_track` gained a new argument `check_duplicates` that allows to the user to specify if temporal duplicates should give an error or not.
- Added `hr_kde` to calculate Kernel home ranges.
- `steps` now uses `difftime` to calcualte time differences.

## minor changes
- Removed: Depends tidyverse
- Fixed errors with lubridate::Periods within `data_frame`s

# amt 0.0.3.0
## minor changes

- Fixed vignette titels.
- Added `Rdpack` to suggest
