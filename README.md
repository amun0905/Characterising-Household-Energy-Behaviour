# Characterising Household Energy Behaviour in the Presence of PV and EV Technologies

**Note:** Due to GitHub's file size limitations, input data is not included in this repository.

---

## Overview

This report investigates how ownership of photovoltaic (PV) systems and electric vehicles (EVs) influences household electricity consumption patterns in the UK. Using aggregated smart meter data from the Smart Energy Research Lab (SERL), the study explores both the level and variability of daily electricity use across different technology ownership groups.

---

## Objectives

- Assess whether PV and EV ownership significantly affects daily electricity consumption and variability.
- Identify statistically significant differences between ownership groups using ANOVA and Tukey HSD tests.
- Apply Principal Component Analysis (PCA) and K-Means clustering to uncover behavioural patterns in energy use.
- Interpret how environmental variables (temperature, solar irradiance, heating degree days) interact with technology ownership.

---

## Methodology

- **Dataset:** Aggregated daily smart meter data from ~13,000 UK households (2020–2023), segmented by heating type, PV, and EV ownership.
- **Preprocessing:** Filtered for gas-heated homes; selected key features (mean, standard deviation, temperature, HDD, solar irradiance); standardised variables.
- **Statistical Analysis:** One-way ANOVA and Tukey HSD to test group-level differences.
- **Unsupervised Learning:** PCA to reduce dimensionality; K-Means clustering (k=3) to identify behavioural clusters.

---

## Key Findings

- **EV ownership** is associated with significantly higher and more variable electricity use.
- **PV ownership** alone has a modest effect on reducing grid electricity use and stabilising demand.
- PCA revealed two dominant axes: one driven by environmental conditions, the other by usage intensity and variability.
- Clustering showed that while technology ownership influences behaviour, it does not fully explain consumption patterns—highlighting the role of other latent factors.

---

## Limitations

- Aggregated data limits granularity and obscures household-level variation.
- Lack of timestamped consumption data restricts temporal analysis.
- PV and EV ownership were the only segmentation variables considered; future work could incorporate demographics and behavioural data.

---

## Suggested Improvements

- Use high-frequency, household-level smart meter data for finer behavioural insights.
- Integrate supervised learning methods to explore causal relationships.
- Expand segmentation to include socio-demographic and behavioural variables.

