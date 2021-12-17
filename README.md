README
================

[![Project Status: Active – The project has reached a stable, usable
state and is being actively
developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
<!-- badges: start -->
[![Lifecycle: stable](https://img.shields.io/badge/lifecycle-stable-brightgreen.svg)](https://www.tidyverse.org/lifecycle/#stable) 
<!-- badges: end -->

# valascotraceR: Validation of a weather driven model to simulate the spread of Ascochyta blight in chickpea over a growing season

The goal of of *valascotraceR* is validate the *ascotraceR* model with independent field data. The model was tested with data from field experiments in which the spatiotemporal spread of Ascochyta blight was investigated from primary infection foci in a susceptible chickpea cultivar (Kyabra) at two different locations: Billa Billa (-28.1011505, 150.3307084) and Tosari (-27.856248, 151.447391), Queensland, Australia. The trial site at both locations had not had chickpea planted on them for over four years, and PreDicta®B tests were conducted to ensure the trial sites were free of _A. rabiei_ DNA. 

## Details of the validation experiments

The trial at Billa Billa was planted on 4 June 2020 and the one at Tosari was planted on 27 June 2020. Briefly, four replicate plots of Kyabra (disease-free seed treated with a Thiram based dressing) were sown in 20 m x 20 m plots on 25 cm row spacing with a seeding rate of 40 seeds per m2. There was a 4.5 m gap between each replicate plots–the gap was sown to wheat buffer to prevent disease spread among chickpea plots. Additionally, a 4.5 m wide buffer of wheat was sown around all four replicate plots to serve as a barrier. 
To initiate primary infections, four naturally infested stubble pieces (each stubble piece was 6–8 cm in length with approximately 80% of area covered by characteristic Ascochyta blight lesions) were placed, in a vertical fashion, at the centre of each newly emerged chickpea plot approximately 14 days after sowing. The selected 1 m2 observation quadrats, marked out at each corner with white pin markers at the distances of 3, 6 and 9 m in a concentric arrangement around the primary infection foci, were checked for the presence or absence of Ascochyta blight infections. The selected quadrats were checked for the presence or absence of Ascochyta blight infections at fortnightly intervals for a total of 10 times at Billa Billa and 8 times at Tosari (disease had spread across whole plots by assessment 8 at Tosari). 
For the entire duration of the experiment, meteorological data was recorded by automated weather stations at the experimental locations

## Comparison of the model prediction vs. observation

In order to validate the model, the model was run with the same start and end dates, field size (20 x 20 m), and seeding rate (40 seeds per m^2) as those of field experiments. The model was run with the weather data recorded at both locations, and the dates of initial infection and number of infected quadrats observed at the time of initial infection were set as observed in the field. All data from this work are included in this repository, and the code used in the statistical analyses and data visualisation is available to run in R Markdown vignettes, including extra instruction for which we did not have space in the paper

The *ascotraceR* model is adapted from a model developed by [(Diggle *et al.*2002)](https://doi.org/10.1094/PHYTO.2002.92.10.1110) for simulating the
spread of anthracnose in a lupin field

## Reference

> Diggle AJ, Salam MU, Thomas GJ, Yang H, O’connell M, Sweetingham M,
> 2002. AnthracnoseTracer: a spatiotemporal model for simulating the
> spread of anthracnose in a lupin field. Phytopathology 92, 1110-21.
