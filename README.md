# ffverse R-Universe

The [ffverse r-universe page](https://ffverse.r-universe.dev) hosts **`stable`** versions of the ffverse set of R packages. 

## Usage

Install specifically from this package repository with:

```r
install.packages('ffscrapr', repo = 'https://ffverse.r-universe.dev')
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

There is a [parallel R-Universe repository](https://dynastyprocess.r-universe.dev) that hosts **`development`** versions of the ffverse R packages.

## ffverse Packages

- [`ffscrapr`](https://ffscrapr.dynastyprocess.com) is an R package for working with FF platform APIs (MFL, Sleeper, Fleaflicker, and ESPN as of right now)
- [`ffsimulator`](https://ffsimulator.dynastyprocess.com) is an R package for simulating fantasy seasons, using historical ADP + nflfastR data + latest FP data.
- [`ffpros`](https://ffpros.dynastyprocess.com) is an R package for accessing FantasyPros.com rankings and projections.

## Roadmap
- `ffverse` is a package that installs and loads all other ffverse packages.
- `ffexpectedpoints` is a package that applies the latest DynastyProcess expected fantasy points models to new nflfastR pbp data.

