# Effect-of-masks-on-the-spread-of-covid-cases

The impact of COVID pandemic has varied globally over
geography and time, as measured by number of cases and
deaths, depending on demographics of the local population
as well as the public health policies implemented in response. 
One such policy response has been is usage of masks
or face covering. Its usage has been very controversial in US
due to perceived impingement over individual freedom.

This programme can be used to understand the impact
of mask policies at local and national scale. Internally, the
tool uses data about COVID19 cases and mask adherence and also applies the emerging technique of Robust Synthetic Control (RSC) (Amjad,
Shah, and Shen 2018) to give counterfactual insights about
how similar regions with different mask decisions diverged
in COVID19 case count.

## Data Used 
COVID19 cases by counties, as per (NYTimes 2020)

## Methodology
The user inputs the state and the target county, along with the time period in question. In preprocessing, counties of the same state with similar trend in Covid cases are considered for the donor pool. The final donor pool will be the target value + counties that did not enact mask mandates. After which RSC is performed to give a counterfactual scenario, where masks were not made mandatory and estimate the percentage difference in the number of Covid cases.
