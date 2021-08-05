## Project List 2021

### Characterising Acoustic Sound Scattering Layers

- Project leads: Nick M
- Presenter: 
- [GitHub](https://github.com/oceanhackweek/ohw21-proj-bioacoustics)

Acoustic data contains information about organisms in the scattering layers. For example, diel vertical migration behavior is visible. This project aims to build tools for classifying and interpreting this data.



### Interactive visualization of open access glider data
- Project leads: Dhruv, Alison
- Presenter:
- GitHub (needs link)

The goal of this project is to show how interactive visualization tools from the [Holoviz ecosystem](https://holoviz.org/) can be combined with glider data access tools ([erddapy](https://github.com/ioos/erddapy), [gliderpy](https://github.com/ioos/gliderpy)) to quickly create a visualization dashboard that can help users intuitively explore glider data.


### CMIP analysis ready data (ARD) workflow : turning big climate projection data into useful inputs for modelling or analysis

- Project leads: Thomas, Paige, Julius
- Presenter: 
- [GitHub](https://github.com/oceanhackweek/ohw21-proj-cmip-ard)

CMIP (Climate Model Intercomparison Project) is a collection of global climate models and is a foundation of global climate projections, helping society better understand the choices we must either make or the impact the communities and industries of our children will face. However there are often barriers (big data, file format, coding familiarity – R vs Python, technical terminology) and challenges (Do I need to dedrift the data? What is this calendar on that model? ) for new users or specific disciplines, such as the marine ecology / ecological modelling community


### Matching open source open environmental data to tagged species data

- Project leads: Jackie
- Presenter:
- [GitHub](https://github.com/oceanhackweek/OHW21_proj_tag_data)

Optimize a tool for making environmental data (ocean velocity, SST) in an easy-to-use format for ecological research (I.e. make mapped data easier to load into R, format data with recognizable variables that are measured by GPS tags)

### Predicting ocean deep currents by satellite data

- Project leads: Iury
- Presenter:
- [GitHub](https://github.com/oceanhackweek/ohw21-proj-deep-currents)

Moorings are expensive and lack long term overage. Deep water oceanography is important. Explore trends & variability from satellites, train a machine learning model to predict deep-water dynamics.


### Pull all ocean repositories in the world to be able to subset

- Project leads: Steve
- Presenter:
- [GitHub] (needs link)

There are so many data repositories already. Hard to search them all. If we wait too long, it will be machine learning solving this for us. 


### High frequency radar data to measure coastal currents

- Project leads: Teresa
- Presenter:
- [GitHub](https://github.com/oceanhackweek/ohw21-proj-coastal-radar)

List of ideas: 

- QC: Use Machine learning methods to filter out interference 
    - PCA to decompose spectrum images into signal and noise components
    - Ensemble averaging over entire bin to factor out range-dependent artifacts for filter development
    - Apply basis transforms in spectral domain to remove broad noise artifacts while preserving sharper features.
- Analyzing surface circulation data to plot circulation along with other datasets


### Use drone imagery of turtles, classify using neural network

- Project leads: Johnathan
- Presenter:
- [GitHub](https://github.com/oceanhackweek/ohw21-proj-drone-turtles)

Use neural networks and pytorch to classify images of turtles. 


### Continue OHW2020 project on OBIS and MPAs

- Project leads: Enrique, Lei
- Presenter:
- [GitHub](https://github.com/oceanhackweek/ohw20-proj-species-marine-protected-areas)

OBIS record from polygons (e.g. MPA or any polygon) together with satellite data & visualize on a map, and select areas, and upload new species abundance data, and do some statistics correlating with MPA properties.


### Adding scale to underwater depth maps from monocular-vision

- Project leads: Yelena Randall
- Presenter:
- [GitHub] (needs link)

Project ideas: 

- Fuse monocular images and IMU data to create scaled depth maps using structure from motion
- Validate using known-size targets that were placed in the underwater scene

Applications:

- Estimation and monitoring coral reef’s volume and surface area.
- Can be used with deep sea vents, rocky reefs, any benthic habitat of interest 
- Estimation of bottom rugosity with important implications for internal waves’ generation.



### Developing pyworms package to improve functionality and usefulness

- Project leads: Diana L-G 
- Presenter:
- [GitHub] (needs link)

Project ideas: 

- Standardizing species names is a key component of sharing and integrating biological data sets
- A Python package already exists to check names against WoRMS, but it has a number of shortcomings:
    - Functions that are incomplete
    - Returns data in a format that is not easily useable by common tools (e.g. pandas)
    - Doesn’t easily handle problems when species names are not matched


### Current/particle back-tracer

- Project leads: Adam K
- Presenter:
- [GitHub] (needs link)

Idea: Provide a tool/package that can take a location on the ocean and a period of time, then back-trace where it would have been at that previous point in time based on winds/currents (this tool might exist). 

Applications: Could be used to re-trace where in-situ samples were taken in open ocean surveys to a common date/time for preserving temporal stationarity in ocean states. 

Motivation: Currents transport plankton, nutrients, fishes in the time it takes a ship to move between samples or as a glider or saildrone passes through it. Most surfaces produced from point observations ignore the drift that occurred between measurements.  This becomes increasingly important when discussing lead-times or lag periods between ocean states and biological observations.


### Determining the degree to which nutrient availability and microbial activity is driven by geologic events

- Project leads: Laura R
- Presenter:
- [GitHub] (needs link)

Project ideas: 

- Use seismic data, elemental data, and phylogenetic analysis/satellite imagery of blooms
- Could help inform what variables are relevant for monitoring geologic activity over time and elucidating how this impacts habitability --could have applications for ocean world exploration (e.g. Enceladus)

- Sampling high-resolution model output as if by an in situ platform (ship, glider, mooring, etc.#ohw21-proj-model-subsampling
- Compare sub-sampled model data to original data to understand what is missed through the sampling
- User-customizable sampling parameters (e.g., ship or glider sampling pattern, depth of sensors, etc.) 
- Would be maybe possible to do this using a wrapper around xarray, as it does have some features to extract non-uniform grid (http://xarray.pydata.org/en/stable/user-guide/interpolation.html#advanced-interpolation would be good starting point).


### SeafloorHUB - Web Aggregator/Python or R package for oceanographic seafloor data 

- Project leads: Stanley
- Presenter:
- [GitHub] (needs link)

Not enough common computational tools regarding data in the deep sea/or coastal marine system. While researchers are interesting in understanding the role of biological pump in the carbon uptake in the ocean, or the contribution of bottom flux from seafloor to the ocean (which fuel upwelling and nutrient regeneration), or the role of trace metal that is fundamentally altering our understanding of the ocean biogeochemical - common open source tools and repo are still behind standard we expect in the field. Often we still use manual ways to find and get the data. I propose we fix that and do it automatically. 

The idea is to create a common hub where all things sediment/seafloor lives. For now I’m thinking of R shiny or other python stack like streamlit/flask. I think of the hub as a mining hub for seafloor data whether you are interested in geochemistry or ecology. You go in and get your data. 



<!-- 
###

- Project leads:
- Presenter:
- [GitHub]()
 -->
