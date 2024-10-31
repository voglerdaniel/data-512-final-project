# Wilfire Impact Estimate in Pueblo, CO

In this analysis, I develop an estimate of smoke intensity from wildfires in Pueblo, CO. I then assess how the smoke intensity score I hypothesize compares to the the Air Quality Index (AQI), a metric commonly used by the US Environmental Protection Agency. 

Thereafter, I then use a seasonal autoregressive integrated moving average (SARIMA) time series model to predict the smoke intensity score I develop 25 years into the future.

Analyses in this repository use data from:
- [Combined wildland fire datasets for the United States and certain territories, 1800s-Present](https://www.sciencebase.gov/catalog/item/61aa537dd34eb622f699df81) dataset, provided by the US Geographic Survey. 
- [EPA Air Quality System (AQS) API](https://aqs.epa.gov/aqsweb/documents/data_api.html)

## Finding Deliverables:
Please find project deliverables in the following locations:
- Visualizations & collaboration reflection at TOP LEVEL OF THIS REPO
- Supprting analysis in the `code/combining_distance_and_aqi.ipynb` file

To review the analysis, please start with `code/fire_distances.ipynb`. That notebook guides users through the remaining workflow.

## Additional Folders
Throughout the notebooks you will find `raw_data` and `intermediate_data` folders referenced. Due to GitHub file size limits the contents of those folders are not included in this repository. If someone were to clone this repository and run the notebooks starting with `code/fire_distances.ipynb`, those folders would be populated locally.