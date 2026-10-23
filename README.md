# Supplementary Data S1

Data, code and results accompanying the manuscript:

**Multivariate hourly weather generation using constrained analogue learning and monthly updating: Evaluation at plateau sites in China**

**Authors:** Ziyi Wang and Jinsong Zhu, Tianjin University.

## Download

- [Download SupplementaryDataS1.zip (138.76 MiB)](https://github.com/six-nut/multivariate-hourly-weather-generation-data/releases/download/v1.0.0/SupplementaryDataS1.zip)
- [Version 1.0.0 release and file details](https://github.com/six-nut/multivariate-hourly-weather-generation-data/releases/tag/v1.0.0)

The release attachment is the original author-supplied `SupplementaryDataS1.zip`, uploaded without repacking or modifying its contents. It contains **1,597 files**. Its size is **145,500,345 bytes** (approximately 139 MiB); the uncompressed files total 255,426,951 bytes. The archive is a release attachment because it exceeds GitHub's 100 MiB limit for a regular Git file.

Download the named attachment above to obtain the numerical data and code. GitHub's automatically generated "Source code" ZIP and TAR.GZ contain only this repository's landing-page files, not the supplementary dataset.

## What is included

The package supports the reconstruction and evaluation of multivariate hourly meteorological histories at five plateau sites in China. Variables include temperature, relative humidity, solar radiation, wind speed and wind direction. It includes native NASA POWER inputs, fitted models, configurations, candidate results, selected histories, figure source data and offline reproduction programs.

After extraction, the archive contains a top-level `SupplementaryDataS1/` directory:

| Directory | Contents |
| --- | --- |
| `record_length/` | Record-length comparisons; the 25-year screening and monthly-updating baseline; next-month evaluation; rolling-output demonstration; inputs, programs, fitted models and result tables. |
| `future_reconstruction/` | Model fitting using the 1995-2024 daily archive, candidate pools, selected 2025-2029 histories and evaluation against withheld January 2025-May 2026 hourly records. |
| `hourly_calibration/` | The 2015 calibration records. |
| `hourly_evaluation/` | The fixed-parameter 2020 conditional hourly test, including donor and boundary-increment records. |
| `site_comparison/` | Descriptors and clustering results for thirteen candidate locations. |
| `main_figures/` | Manuscript figures, editable figure files and panel-level source data. |
| `README.md` | Package overview, reproduction commands and mapping of files to manuscript tables and figures. |

Manuscript sites P1-P5 (Qingshuihe, Nagqu, Shigatse, Nyingchi and Golmud) correspond to source-file identifiers C1, P1, P2, P3 and P4, respectively. These are alternative labels for the same numerical data.

## Reproduction and interpretation

Use Python 3.12 and the requirements supplied in each numerical directory. The bundled documentation records the software environment, input units, time conventions, seeds, processing stages and evaluation definitions. Computations can run offline using the supplied inputs.

The main reproduction instructions are in:

- `SupplementaryDataS1/README.md`
- `SupplementaryDataS1/record_length/README.txt`
- `SupplementaryDataS1/record_length/docs/PROTOCOL.md`
- `SupplementaryDataS1/future_reconstruction/README.md`

Daily inputs use local solar time (LST), and delivered hourly histories use China Standard Time (CST, UTC+8). Follow the directory-specific documentation for units and donor time offsets. In particular, relative humidity is percent in hourly CSV files and a fraction in the five-factor `.dat` files.

The selected 2025-2029 histories are statistically representative meteorological inputs under a prescribed temperature scenario. They are not forecasts of individual future weather events.

## Provenance and reuse

NASA POWER input data remain subject to the conditions of the [NASA POWER project](https://power.larc.nasa.gov/). The archive retains original request URLs and retrieval metadata. Its supplied README states that the package is provided for peer review and reproduction of the results. This repository does not add a new data or software licence to the supplied package.

## Dataset citation

Wang, Z. and Zhu, J. (2026). *Supplementary Data S1: Multivariate hourly weather generation using constrained analogue learning and monthly updating: Evaluation at plateau sites in China*, version 1.0.0. GitHub. https://github.com/six-nut/multivariate-hourly-weather-generation-data/releases/tag/v1.0.0

Use the versioned release URL when citing this deposit. No DOI has been assigned to this GitHub release.

## Data availability text

The data and code supporting this study are available in Supplementary Data S1 (version 1.0.0) at https://github.com/six-nut/multivariate-hourly-weather-generation-data/releases/tag/v1.0.0. The archive includes NASA POWER inputs, analysis code, fitted models, generated meteorological histories, evaluation results and figure source data.
