# Wilfire Impact Estimate in Pueblo, CO

In this analysis, I develop an estimate of smoke intensity from wildfires in Pueblo, CO. I then assess how the smoke intensity score I hypothesize compares to the the Air Quality Index (AQI), a metric commonly used by the US Environmental Protection Agency. 

Thereafter, I then use a seasonal autoregressive integrated moving average (SARIMA) time series model to predict the smoke intensity score I develop 25 years into the future.

Analyses in this repository use data from:
- [Combined wildland fire datasets for the United States and certain territories, 1800s-Present](https://www.sciencebase.gov/catalog/item/61aa537dd34eb622f699df81) dataset, provided by the US Geographic Survey. 
- [EPA Air Quality System (AQS) API](https://aqs.epa.gov/aqsweb/documents/data_api.html)

## Finding Deliverables:
Please find project deliverables in the following locations:
- Key figures are in the `output` folder, located [here](./output/)
- Discussion on the primary insights from the figures are in the `visualizations_and_reflections.pdf` report [here](./visualizations_and_reflections.pdf)
- Reflections on the collaborative efforts that produced the analysis behind these figures is in the `collaborative_reflection_statement.docx` [here](./collaborative_reflection_statement.docx)

Notebooks documenting the analysis that led to the above outputs is contained in the `code` folder [here](./code/). The analysis is divided into four different notebooks, one for each major stage of work:
- **Notebook 1:** [Calculating Fire Distances](./code/fire_distances.ipynb) calculates the distance between in-scope wildfires and Pueblo, CO 
- **Notebook 2:** [Getting AQI Data](./code/getting_aqi.data.ipynb) gathers the constituent parts of air quality index (AQI) and uses them to calculate the index
- **Notebook 3:** [Combining Distance and AQI](./code/combining_distance_and_aqi.ipynb) computes the smoke intensity estimate (SIE) metric using the distances from Notebook 1, then analyzes its association with the AQI index.
- **Notebook 4:** [Public Health Extension](./code/public_health_extension.ipynb) explores variables quantifying public health outcomes provided by the Colorado Dept. of Public Health & Environment; analyzes and visualizes their association with the SIE.

## Additional Folders
Throughout the notebooks you will find `raw_data` and `intermediate_data` folders referenced. Due to GitHub file size limits the contents of those folders are not included in this repository. Please clone this repository and run the notebooks starting with `code/fire_distances.ipynb` to populate these folders locally.

**EXCEPTION**: the `raw_data` folder contains [a subfolder](./raw_data/colorado_epht_data/) with the original data provided by the Colorado Department of Public Health and Environment. Colorado does not make this data available via an API, so it is included in this repository in its original format.