# VRES paper

This is the repository for the paper "Meteorological drivers of extreme renewable energy shortage events in Germany and their sensitivity under climate change"

Abstract:

The pursuit of a climate-neutral future accelerates the expansion of renewable energy
sources such as wind and solar power. A key challenge for these technologies is their
sensitivity to weather variability. Periods of extremely low renewable energy production
coinciding with high demand, so-called variable renewable energy shortages (VRES), are
especially critical for grid stability. VRES are commonly studied with observational data,
which only represent one possible realisation of internal climate variability and are
therefore not sufficient to adequately study extreme VRES. Additionally, the effect of
non-stationarity under climate change on VRES is only starting to be investigated and is
not yet fully understood. In this study, we evaluate a simple energy model for Germany
using ERA5 reanalysis data and apply it to 3840 years of climate data from different
Earth System Models (ESMs) under current climate and in a climate with +2 K global
warming. We analyse the model outputs with regard to seasonality, event magnitude,
duration, composition, and large-scale weather regimes. We find that VRES events exhibit
a pronounced seasonality, with both occurrence and magnitude peaking in mid-winter. We
identify variability in wind speed over Germany as the main driver of these events, while
fluctuations in incoming solar radiation contribute only marginally during the winter
months. The most extreme physically plausible VRES derived from ESM data are up to
6.11 % (1-day events), 8.83 % (7-day events), and 10.44 % (14-day events) more severe
than those observed in the same climate period. The energy production only changes
marginally under warming conditions, while the demand is decreasing due to higher winter
temperatures. This results in decreasing VRES event numbers while the magnitude of
potential worst-case events remains extreme. In addition, a bottom-up weather pattern
clustering analysis identifies different blocked circulation regimes as a dominant driver in
the formation of VRES over Germany. Among the weather patterns leading to VRES
events, two blocking patterns are particularly relevant for longer-lasting VRES events due
to their particularly cold temperatures over Germany. These results provide energy system
planners with robust worst-case benchmarks for VRES severity under current and future
warming and contribute to a deeper understanding of the climatic drivers behind periods
of renewable energy shortfall.

Link to the paper: will be posted here

## Info

0. Download data

    - Use dl_CMIP6.ipynb - CMIP6 data is available publicly from the ESGF https://pcmdi.llnl.gov/CMIP6/
    - dl_CESM_LE_{var}.py - CESM2 Large Ensemble data is available publicly from the GDEX https://gdex.ucar.edu/datasets/d651056/
    - dl_ERA5_{var}.py - ERA5 data is available publicly from the CDS https://cds.climate.copernicus.eu/datasets/reanalysis-era5-single-levels?tab=overview
    - German capacity data is available publicly from the MaStR https://www.marktstammdatenregister.de/MaStR/Datendownload under the dl-de/by-2-0 license (http://www.govdata.de/dl-de/by-2-0).
    - ENTSO-E data for Germany is available publicly from the SMARD data portal https://www.smard.de/home/downloadcenter/download-marktdaten/
    - Postcode data (used for spatial aggregation) is available publicly from ESRI ArcGIS Hub https://hub.arcgis.com/datasets/esri-de-content::postleitzahlengebiete-in-deutschland/explore?location=51.164397\%2C10.454123\%2C7
    - Population data (used for temperature weighting) is available publicly from Earth Data https://www.earthdata.nasa.gov/data/catalog/sedac-ciesin-sedac-gpwv4-popdens-r11-4.11
    - Global temperature data is available publicly from Berkeley Earth https://berkeleyearth.org/data/; GISTEMP https://data.giss.nasa.gov/gistemp/; Hadcrut https://www.metoffice.gov.uk/hadobs/

1. Calculate warming periods for the ESMs (01_Annual_Temperatures)
2. Preprocess and analyse variables (02_Var_Preprocessing_and_analysis)
3. Prepare simple energy model (preprocess capacity data etc.) (03_SEM_Preparation)
4. Calibrate the SEM and run it for different datasets (04_SEM_application)
5. Combine the different results for analysis (05_Post_processing)
6. Analyse the model outputs (06_RL_Analysis)
7. Detect VRES events and analyse the results (07_VRES_Detection_and_Analysis)
8. Perform a psl clustering and analyse the results (08_PSL_clustering)



## Authors:

Onno Nennecke, Dr. Peter Pfleiderer and Jun.-Prof. Dr. Sebastian Sippel  
Institute for Meteorology
Faculty of Physics and Earth System Sciences  
Leipzig University

## Contact

Onno Nennecke: [onno.nennecke@uni-leipzig.de](onno.nennecke@uni-leipzig.de)

# License
[MIT](https://github.com/O-Nennecke/Nennecke_et_al_2026/blob/main/LICENSE)
