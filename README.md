# ffverse R-Universe

The [ffverse r-universe page](https://ffverse.r-universe.dev) hosts **`development`** versions of the ffverse set of R packages. 

## Usage

Install specifically from this package repository with:

```r
install.packages('ffscrapr', repo = c('https://ffverse.r-universe.dev', getOption('repos')))
```

You can also default-enable this repository by adding the following option to [your R profile](https://usethis.r-lib.org/reference/edit.html) before installing any ffverse package: 

```r

options(
  repos = c(
    ffverse = 'https://ffverse.r-universe.dev',
    CRAN = 'https://cloud.r-project.org'
  ))

install.packages('ffscrapr')
```

## ffverse Packages

- [`ffscrapr`](https://ffscrapr.ffverse.com) is an R package for working with FF platform APIs (MFL, Sleeper, Fleaflicker, and ESPN as of right now)
- [`ffsimulator`](https://ffsimulator.ffverse.com) is an R package for simulating fantasy seasons, using historical ADP + nflfastR data + latest FP data.
- [`ffpros`](https://ffpros.ffverse.com) is an R package for accessing FantasyPros.com rankings and projections.
- [`ffopportunity`](https://ffopportunity.ffverse.com) is a package that applies the latest ffverse expected fantasy points models to new nflfastR pbp data.
- 
## Roadmap
- `ffverse` is a package that installs and loads all other ffverse packages.
