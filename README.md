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

## Sources and Citations
