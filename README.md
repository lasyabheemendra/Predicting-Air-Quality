# Predicting-Air-Quality



This directory contains the work done by all team members of Group 9 towards the term project. This document can be used as a README file and will describe the different files present here along with the purposes they serve.

Dataset:
The dataset has been divided into 5 sections, each of which is devoted to a pollutant. The daily summary data of each pollutant for the years 2000-2020 has been uploaded to the following five sub directories. They collectively form the dataset for the project.
1.	FA21 CMPE 255 Term Project/CO
2.	FA21 CMPE 255 Term Project/SO2/data
3.	FA21 CMPE 255 Term Project/NO2
4.	FA21 CMPE 255 Term Project/Ozone
5.	FA21 CMPE 255 Term Project/PM2.5/data

US Census data for population estimates: FA21 CMPE 255 Term Project/co-est2020.csv
EPA site data for land use and location setting: FA21 CMPE 255 Term Project/aqs_sites.csv  

Preprocessing and prediction code Files:
Within each of the aforementioned subdirectories, colab files/ipynb files are present which contain the source code used to preprocess the data and to generate the AQI for test data(years 2018-2020). File paths are as follows:
1.	FA21 CMPE 255 Term Project/CO/CO_GradientBoost.ipynb 
2.	FA21 CMPE 255 Term Project/NO2/NO2LinearRegression.ipynb
3.	FA21 CMPE 255 Term Project/Ozone/OzoneGradientBoost.ipynb
4.	FA21 CMPE 255 Term Project/PM2.5/PM2.5GradientBooster.ipynb.ipynb
5.	FA21 CMPE 255 Term Project/SO2/SO2_GradientBooster_AQI.ipynb

Prediction files for test data:
Within each of the pollutant subdirectories, the AQI prediction files are also contained.
1.	FA21 CMPE 255 Term Project/SO2/SO2_AQI_Predicted 
2.	FA21 CMPE 255 Term Project/PM2.5/PM2.5_AQI_Predicted
3.	FA21 CMPE 255 Term Project/Ozone/Ozone_AQI_Predicted
4.	FA21 CMPE 255 Term Project/NO2/NO2_AQI_Predicted
5.	FA21 CMPE 255 Term Project/CO/CO_AQI_Predicted

AQI prediction processing files:
The following files have been used to explore the predicted AQI for all five pollutants. The data is processed differently in each file and has been used iteratively to build the visualizations for this project. The files and their processing steps is detailed below:
1.	FA21 CMPE 255 Term Project/Combined Pollutants/PollutantMerge_ver1.ipynb
Initial analysis to generate visualizations. The mean of AQI per month was calculated and the resulting dataset was merged with population and site information to draw up graphs. These graphs were used to analyze associations between the different datasets.
Result file: FA21 CMPE 255 Term Project/Combined Pollutants/PredictedAQIData.csv
Associated visualization (not most recent): FA21 CMPE 255 Term Project/Visualizations/AQI_Visualization_Subset.twbx

2.	FA21 CMPE 255 Term Project/Combined Pollutants/PollutantMerge_final.ipynb
Modified version of PollutantMerge file, to address bugs in processing which did not generate accurate visualizations. In this file, the mean of AQI over a month is not calculated.
Result file: FA21 CMPE 255 Term Project/Combined Pollutants/predictedQualityWithSite1.csv
Associated visualization: FA21 CMPE 255 Term Project/Visualizations/AQIDays1.twbx

Association Analysis:
Association Analysis has been performed and the code files for train and test data can be found as detailed below: 
Train data: FA21 CMPE 255 Term Project/Association Analysis/AssociationAnalysis_TrainData.ipynb
Test data: FA21 CMPE 255 Term Project/Association Analysis/AssociationAnalysis_predictedData.ipynb

Comparing different Algorithms:
Before selecting Gradient Boosting Regressor, few other algorithms were tested for PM2.5 and SO2 pollutants. Below files show the results obtained from it.
1.	FA21 CMPE 255 Term Project/PM2.5/PM2.5_algorithms_AQI.ipynb
2.	FA21 CMPE 255 Term Project/SO2/SO2_algorithms_AQI.ipynb

The comparison of different algorithms for other pollutants was included within these files:
3.	FA21 CMPE 255 Term Project/CO/CO_GradientBoost.ipynb 
4.	FA21 CMPE 255 Term Project/NO2/NO2LinearRegression.ipynb
5.	FA21 CMPE 255 Term Project/Ozone/OzoneGradientBoost.ipynb

