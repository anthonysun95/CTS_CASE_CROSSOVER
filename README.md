# A tutorial on the case time series design for small-area analysis

### Brief introduction

**CTS design**: The case time series design was introduced by Antonio Gasparrini in 2021 to address the challenge brought by intensive longitudinal and big data settings. The CTS is a combination of time series and traditional self-matched method.

**Case crossover design**: was introduced by Malcolm Maclure in 1991. In 2005, Holly Janes compared different temporal settings in case crossover design and recommended the time stratified approach because it ensured unbiased estimates avoiding overlap bias and time trend bias. Recently, Yuming Guo extended the approach to a space-time-stratified case crossover to accommodate the multilocation studies. 


------------------------------------------------------------------------

CTS and case crossover could be both applied at individual level and small geographic scale level. This repository provides review and application for both study designs. References are presented below: 

Gasparrini A. A tutorial on the case time series design for small-area analysis. BMC Med Res Methodol. 2022;22(1):129. doi:10.1186/s12874-022-01612-x

Wu Y, Li S, Guo Y. Space-Time-Stratified Case-Crossover Design in Environmental Epidemiology Study. Health Data Science. 2021. doi:10.34133/2021/9870798

Gasparrini A. The Case Time Series Design. Epidemiology. 2021;32(6):829-837. doi:10.1097/EDE.0000000000001410

Maclure M. The case-crossover design: a method for studying transient effects on the risk of acute events. Am J Epidemiol. 1991;133(2):144-153. doi:10.1093/oxfordjournals.aje.a115853

Janes H, Sheppard L, Lumley T. Case-crossover analyses of air pollution exposure data: referent selection strategies and their implications for bias. Epidemiology. 2005;16(6):717-726. doi:10.1097/01.ede.0000181315.18836.9d

### Data

**Individual CTS and case crossover**: The data was simulated by Antonio and included 1,601 subjects who reported daily the occurrence of respiratory symptoms such as asthma and allergic rhinitis in a smartphone app, and who were assigned exposure levels by linking their geo-located position with high-resolution spatio-temporal maps of pollen, air pollution, and temperature. Anthony added codes for an individual time-stratified case crossover study design following the CTS design.

**Small-area CTS and space-time-stratified case crossover**: The data used in this case study are generated from Antonio Gasparrini's paper - "A tutorial on the case time series design for small-area analysis". The case study describes an analysis on the association between heat and mortality in two summers (2006 and 2013) in London, UK. The data are provided for 983 middle layer super output areas (MSOAs), which are small census-based aggregations. The mortality data is then linked with gridded daily temperature data, and then with measures of area-level deprivation at lower layer super output areas (LSOAs).


Specifically, the folder *data* includes the following datasets:

-  *london_mortality.rds*: R data file storing the number of deaths and daily mean temperaturefor each MSOA of London in each day, for two age groups.


### R code and PDF output

The two R scripts reproduces all the steps of the analysis using CTS and case crossover design. Specifically:

-   *individualCTS_CC.Rmd* individual CTS and case crossover study
-   *individualCTS_CC.pdf* output from "individualCTS_CC.Rmd"
-   *aggregatedCTS_CC.Rmd* small-area CTS and space-time-stratified case crossover study
-   *aggregatedCTS_CC.pdf* output from "aggregatedCTS_CC.Rmd"



### Terms of use

The use of data follows GNU public licence, which permits commercial use, modification, distribution, patent use and private use. 


