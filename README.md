# Delta Smelt Distribution Data
This repository contains data describing Delta Smelt distribution in the Delta from 1995-2015

# Data Format
The `DS_distribution_JanDec_1995_2015.txt` is a matrix. Rows represent time (months) and columns 3-14 represnt regions. Each row contains a month, year, and the observed occupancy probabilities of regions studied. Columns 1 and 2 indicate the year and month, respectivley. Data for the 12 spatial strata are ordered Sacramento R., South Delta, East Delta,
Lower Sacramento R., Lower San Joaquin R., Confluence, SE Suisun, NE Suisun, Suisun Marsh, SW Suisun, NW Suisun, Yolo Bypass.

# Methods for Preparing Fish Distribution Data for Model Input 
by Will Smith 

Observed delta smelt distributions DS<sub>yms</sub> were developed from 20-mm, Midwater Trawl, and Spring Kodiak Surveys.
Townet Survey data were not used, because tow volume data were unavailable before 2003, use of Townet data would only leverage one additional 
month of distribution information (August), and in most year-months with a concurrent 20-mm Survey sample, delta smelt were observed in fewer
spatial strata in the Townet Survey (in 7 of 13 years). Fish survey data were made available online by [CDFW](ftp://ftp.dfg.ca.gov/). 
Monthly observed catch densities (catch/volume sampled) were assigned to the 12 spatial strata, and observed densities were expanded to total 
population abundance by multiplying by strata volumes. Strata volumes were estimated by Derek Hilts using DSM2. Estimated population abundances 
in each spatial stratum were then converted to proportions of the total abundance, which were interpreted as observed occupancy probabilities.

Surveys were not completed in all months, and in some months, no fish were observed (mostly February, March, and August). Distributions from
the prior month were assumed when observations were missing. A high level of zero-inflation, resulting in zero observed occupancy of many spatial 
strata, was noted beginning in spring of 2015; therefore, the terminal cohort of observed spatial distributions was 2014 (last observed in April 2015). 

Delta smelt densities in the South Delta stratum were depleted by entrainment, resulting in a negative bias and underestimation of the proportion
of the population in this region of the Delta. Observed South Delta densities were therefore divided by estimates of proportional entrainment loss 
(Smith et al. 2021) to correct for bias.
