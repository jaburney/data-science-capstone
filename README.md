# Data Science Capstone
### Land Use Change Dynamics

Fall Quarter (2021)

Please make sure to do the listed tasks *for* that week's class meeting.

--- 
**Week 1** - Introduction to land-use change.

What do we mean by land use? Land use change? How do we measure these quantities using satellite remote sensing imagery?

+ NASA primer on [remote sensing](https://appliedsciences.nasa.gov/sites/default/files/D1P3_Fundamentals.pdf).
+ NASA primer on [measuring vegetation from space](https://earthdata.nasa.gov/learn/pathfinders/biodiversity/vegetation-characteristics).
+ Hansen, et. al. *Science* (2013) [High-Resolution Global Maps of 21st-Century Forest Cover Change](https://storage.googleapis.com/pub-tools-public-publication-data/pdf/42119.pdf).
+ Burke & Lobell. *PNAS* (2017) [Satellite-based assessment of yield variation and its determinants in smallholder African systems](https://www.pnas.org/content/114/9/2189).

---
**Week 2** - Introduction to Google Earth Engine and Colab Interface

Google Earth Engine contains a huge amount of processed satellite imagery and reflectance data stored as latitude-longitude raster data. This quarter, we will use Google Colab for ease of interface with these data sources. This week, you need to get yourself set up to use Earth Engine data by doing the following:

1. Get yourself a Google Earth Engine account with your ucsd.edu email address. This may take a day or so to confirm so don't wait until the last minute
2. Work through [this tutorial](https://colab.research.google.com/github/google/earthengine-api/blob/master/python/examples/ipynb/ee-api-colab-setup.ipynb) to link your earth engine account to your Colab/Drive. Step through the tutorial to understand some of the basic Earth Engine functionality.
3. Create your own Colab file for this quarter. Set it up for Earth Engine API access, and familiarize yourself with the basic structure of [Image Collections in Earth Engine](https://colab.research.google.com/github/csaybar/EEwPython/blob/master/3_eeImageCollection.ipynb).
5. Read about the structure of [surface reflectance data from Sentinel 2](https://developers.google.com/earth-engine/datasets/catalog/COPERNICUS_S2_SR).
6. Load in the Sentinel 2 land surface reflectance image collection and map the a recent Red Edge 1 band image for the globe.

For the future, you can also access Earth Engine data and commands via your own python installation ([see here](https://developers.google.com/earth-engine/guides/python_install)). 

---
**Week 3** - Vegetation Indices, Time Averaging

Please read about Vegetation Indices:

* [NDVI](https://en.wikipedia.org/wiki/Normalized_difference_vegetation_index)
* [NASA Earth Observation Data for Vegetation Monitoring](https://earthdata.nasa.gov/earth-observation-data/near-real-time/hazards-and-disasters/vegetation)
* [Other vegetation indices](https://eos.com/blog/6-spectral-indexes-on-top-of-ndvi-to-make-your-vegetation-analysis-complete/)

For this week:
1. Choose a region of interest for your vegetation study.
2. Choose an appropriate vegetation index for your region of interest.
3. Generate your VI data montly for 2020 (average for each month). You will want to read about band and time reducers [here](https://colab.research.google.com/github/csaybar/EEwPython/blob/master/5_Reducer.ipynb).
4. Make a figure, set of figures, or animation of your monthly data using a interactive map. (More on [interactive maps in Python with Folium](https://www.earthdatascience.org/courses/scientists-guide-to-plotting-data-in-python/plot-spatial-data/customize-raster-plots/interactive-maps/).)

---
**Week 4** - Cloud Screening and Quality Control

Please complete [this cloud masking tutorial](https://developers.google.com/earth-engine/tutorials/community/sentinel-2-s2cloudless).

Add cloud masking to your region of interest study. Can you figure out how many images are being used per pixel for each monthly value?

Questions for this week: 
+ Why do you think cloud masking is important?
+ How might your analysis be biased by clouds?

---
**Week 5** - Feature Classes (Spatial Summaries)

Read about [Feature Classes](https://colab.research.google.com/github/csaybar/EEwPython/blob/master/4_features.ipynb) and [Spatial Reducers](https://colab.research.google.com/github/csaybar/EEwPython/blob/master/5_Reducer.ipynb).

Your goal this week is to calculate mean, minimum, and maximum VI values for your region of interest, aggregated over administrative boundaries.

---
**Week 6** - Trend Analysis

This week, write code to calculate trends in vegetation indices both as rasters (plot this), and aggregated over administrative boundaries. There are several ways to do this, including exporting to data frame. 

---
**Week 7** - Ramp-Up Summary

This week is a moment to review, perhaps go back and revise or tweak your analysis, comment your code, and add some presentation flair to your ramp-up analysis.

---
**Week 8** - Proposal Ideas

Come prepared to talk project ideas with the group. 

---
**Week 9** - No meeting (Thanksgiving)

---
**Week 10** - Proposal Pitch and Schedule

I look forward to seeing your plans!
