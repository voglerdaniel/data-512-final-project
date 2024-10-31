# Wilfire Impact Estimate in Pueblo, CO

In this analysis, I develop an estimate of smoke intensity from wildfires in Pueblo, CO. I then assess how the smoke intensity score I hypothesize compares to the the Air Quality Index (AQI), a metric commonly used by the US Environmental Protection Agency. 

Thereafter, I then use a seasonal autoregressive integrated moving average (SARIMA) time series model to predict the smoke intensity score I develop 25 years into the future.

Analyses in this repository use data from:
- [Combined wildland fire datasets for the United States and certain territories, 1800s-Present](https://www.sciencebase.gov/catalog/item/61aa537dd34eb622f699df81) dataset, provided by the US Geographic Survey. 
- [EPA Air Quality System (AQS) API](https://aqs.epa.gov/aqsweb/documents/data_api.html)

## Finding Deliverables:
Please find project deliverables in the following locations:
- Collaboration reflection at the top level of this repo
- Visualizations PDF in the `output` folder
    - Reflections on each visualization are in that document and in the `code/combining_distance_and_aqi.ipynb` file

To review the analysis, please start with `code/fire_distances.ipynb`. That notebook guides users through the remaining workflow.