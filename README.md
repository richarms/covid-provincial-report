# covid-provincial-report

This report summarises the results of an epidemiological model to estimate the near-term upper and lower bounds for total demand for hospitalization per province in South Africa due to COVID-19, to aid with production and logistics planning for the National Ventilator Project executed by SARAO.

In our National Model work, we provide long-range (1-year) national forecasts by varying  𝑅𝑡  over plausible values intended to capture both goverment social interventions and heterogenous social compliance, within a still-unknown epidemiological landscape.

Here, we instead use the near-past to predict the near-future: for each independent provincial model, we fit an exponential function to the previous 14 days of case data, and run 1000 scenarios, where the value of  𝑅𝑡  is allowed to vary within the standard deviation of this fit. Importantly, model are instantiated with current reported data, and thus predict future reported parameters. Ensembles are reported with 68 percentile confidence intervals, as well as histograms through the ensembles at a 30-day horizon.

Our models have several limitations. We rely on data from https://github.com/dsfsi/covid19za. We assume no inter-provincial mixing. We do not model heterogenous infectivity, such as 'superspreader' scenario effects, unknown community immunity, etc. These are short-term models: long-term predictions should take in to account government interventions and community compliance on the effective values  𝑅𝑡(𝑡)  can assume.

__

Disclaimer: the models described here are intended for general information purposes only. The authors accept no liability or responsibility for the use of the information in this document and provide no warranty regarding any results, data or code herein.
