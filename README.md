# Monarch Butterfly Convolutional Neural Network Species Distribution Models (CNN-SDMs)
Welcome to my Maker Portfolio!

## Description
This project trains and evaluates 5 monarch butterfly CNN-SDMs, each corresponding to a temporal and regional stage of the multi-generational migration route:
1. Spring (Mar-May, Southern U.S.)
2. Summer (May-Aug, Northern U.S.)
3. Fall North (Sep-Nov, Northern U.S.)
4. Fall South (Sep-Nov, Southern U.S.)
5. Winter (Nov-Mar, Mexico)

This project has two major parts: 

First, CNN-SDM training, performance evaluation, and permutation importance analysis are performed in the code files under the `src/creating_models/` folder. 

Second, future climate and land cover conditions are projected onto each CNN-SDM, followed by mapping future distributions and analyzing feature importance with SHAP (SHapley Additive exPlanations) values. Code files for this step are found under the `src/future_projections/` folder.

Methodological details are documented within the code comments. For the complete study, refer to the published paper in the _Journal of Dawning Research_: https://dawningresearch.org/Papers/2025/JDR2025Article07.pdf

## Downloading Data and Running Code
All code can be run directly on Google Colab after downloading the required data files below.

*Note: Random seeds were not fixed in this study, so your results may show minor variations from those reported in the paper and in the Google Colab notebook outputs.*

### Creating Models Code
Train/test data for each CNN-SDM are named according to their group: Spring, Summer, Fall North (abbreviated fall_n), Fall South (abbreviated fall_s), Winter

https://drive.google.com/drive/folders/1L7OcwWVItt6bOmoZY38200yCcmez8I-3?usp=sharing

### Future Projections Code
CNN-SDM Models (or you can use the model you trained yourself from the first step)

https://drive.google.com/drive/folders/1SdXJEhKILZaszX_5TyJEfcc1M9388eGc?usp=sharing

Model inputs for future climate and land cover conditions are named according to the group and Shared Socioeconomic Pathway and Representative Concentration Pathway (SSP-RCP) scenario

https://drive.google.com/drive/folders/1HUNx0qUm9IPDBB7lgzfJeLsswD1RsuzU?usp=sharing

Map boundary visualization data for future distribution plots

https://drive.google.com/drive/folders/1zjs8Yu6l0mKh64Tb2qqRQmd5jfVvQe8R?usp=sharing

Model training data, named according to the group, for SHAP background data

https://drive.google.com/drive/folders/15GdfUJj-B17jnfBnfLQZPNX8LFjUaDob?usp=sharing

## Data Sources
* Global Biodiversity Information Facility Monarch Butterfly (Danaus plexippus) Occurrence Data: https://doi.org/10.15468/dl.ybejfm
* WorldClim Elevation Data: https://www.worldclim.org/data/worldclim21.html
* WorldClim Historical Monthly Weather Data: https://www.worldclim.org/data/monthlywth.html
* United States Geological Survey (USGS) National Water-Quality Assessment (NAWQA) Pesticide National Synthesis Project County-Level Glyphosate Use Data: https://water.usgs.gov/nawqa/pnsp/usage/maps/county-level/
* Land-Use Harmonization 2 (LUH2) v2h Release Land Cover Data: https://luh.umd.edu/data.shtml
* WorldClim Future Climate Data from Hadley Centre Global Environment Model (HadGEM3) for 2061-2080: https://www.worldclim.org/data/cmip6/cmip6_clim10m.html
* Land-Use Harmonization 2 (LUH2) v2f Release Future Land Cover Projections: https://luh.umd.edu/data.shtml

## Methodology Bibliography
### Migration Stages Grouping

Oberhauser, K., Wiederholt, R., Diffendorfer, J. E., Semmens, D., Ries, L., Thogmartin, W. E., Lopez-Hoffman, L., & Semmens, B. (2016). A trans-national monarch butterfly population model and implications for regional conservation priorities. *Ecological Entomology, 42*(1), 51–60. https://doi.org/10.1111/een.12351

Flockhart, D. T. T., Wassenaar, L. I., Martin, T. G., Hobson, K. A., Wunder, M. B., & Norris, D. R. (2013). Tracking multigenerational colonization of the breeding grounds by monarch butterflies in eastern North America. *Proceedings of the Royal Society B: Biological Sciences, 280*(1768), 20131087. https://doi.org/10.1098/rspb.2013.1087

### Surface Range Envelope (SRE) Pseudo-Absence Generation Method
Barbet-Massin, M., Jiguet, F., Albert, C. H., & Thuiller, W. (2012). Selecting pseudo-absences for species distribution models: how, where and how many? *Methods in Ecology and Evolution, 3*(2), 327–338. https://doi.org/10.1111/j.2041-
210x.2011.00172.x

### CNN-SDM Architecture
Deneu, B., Servajean, M., Bonnet, P., Botella, C., Munoz, F., & Joly, A. (2021). Convolutional neural networks improve species distribution modelling by capturing the spatial structure of the environment. *PLOS Computational Biology, 17*(4), e1008856. https://doi.org/10.1371/journal.pcbi.1008856

Deneu, B., Joly, A., Bonnet, P., Servajean, M., & Munoz, F. (2022). Very High Resolution Species Distribution Modeling Based on Remote Sensing Imagery: How to Capture FineGrained and Large-Scale Vegetation Ecology With Convolutional Neural Networks? *Frontiers in Plant Science, 13*, 839279. https://doi.org/10.3389/fpls.2022.839279
