# Machine-Learning-Guided Band-Edge Prediction of Halide Double Perovskites

## Overview

This repository contains supplementary data for the research paper:

**“Machine-learning guided prediction of band edge energies of halide double perovskites for design of efficient perovskite solar cells.”**

The study develops a machine-learning framework to predict the valence band maximum (VBM) and conduction band minimum (CBM) of halide double perovskites with the general chemical formula A₂B′B″X₆. The research aims to support high-throughput screening and the discovery of promising lead-free photovoltaic absorber materials.

## Repository Contents

The supplementary document `Supplementary_Tables_.docx` contains Tables S1–S4:

- **Table S1:** Complete 1,000-entry model-development composition list, with standardized A₂B′B″X₆ formulas and source IDs.
- **Table S2:** Training-set membership for the final 85:15 train–test split.
- **Table S3:** Internal test-set membership for the final 85:15 train–test split.
- **Table S4:** Revised six-compound composition-level out-of-sample validation set, including predicted and literature-reported CBM and VBM values.

The final dataset partition was reproduced using `train_test_split(test_size=0.15, random_state=42, shuffle=True)`.

## Key Results

The manuscript reports the following performance for the stacking ensemble model using the 85:15 train–test split:

| Target property | R² | RMSE (eV) | MAE (eV) |
|---|---:|---:|---:|
| Valence band maximum (VBM) | 0.8540 | 0.2204 | 0.1720 |
| Conduction band minimum (CBM) | 0.8619 | 0.2136 | 0.1556 |

The trained models were applied to a combinatorial library of 5,418 candidate compositions, followed by structural, environmental, economic, and band-gap screening to identify promising lead-free double-perovskite candidates.

## Purpose of the Supplementary Data

These tables are provided to improve transparency and reproducibility by documenting the model-development compositions, exact training and internal test memberships, and the independent composition-level validation set described in the manuscript.

## Data Format

- **File format:** Microsoft Word (`.docx`)
- **Document:** `Supplementary_Tables_.docx`


## Notes

- The supplementary tables document the dataset membership and validation information associated with the manuscript.
- The reported model-performance values are taken from the manuscript.
- The supplementary document is intended to be read alongside the associated research article.
- Please consult the manuscript for the complete methodology, model details, screening criteria, and interpretation of the results.

## Contact

For questions regarding the supplementary data, please contact the corresponding author listed in the associated research article.
