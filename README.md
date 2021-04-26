# SultzerSwit_ENV872_EDA_FinalProject
This is a way to organize our final project for Environmental Data Analytics Spring 2021

## Summary

The purpose of this document is to provide background information for the repository containing the Data Analytics project conducted by Kendra Sultzer and Nadia Swit in the spring of 2021.  This project focused on analyzing the trends within manure management for livestock in the United States. Analysis goals included identifying how methane emissions have changed over time and how methane emissions over time are different between different livestock.This repository contains datasets, code, project files, and presentation files.  

## Investigators

* Kendra Sultzer, Duke Nicholas School of the Environment's Master of Environmental Management Candidate 2021, kendrasultzer@gmail.com, co-author  

* Nadia Swit, Duke Nicholas School of the Environment's Master of Environmental Management Candidate 2022, nadswit@gmail.com, co-author

## Keywords

manure, manure management, methane, livestock emissions, green house gases, GHG

## Database Information

Data for this project was obtained from the United Nation's Food and Agriculture Organization (FAO).  Specifically, this information is from FAOSTAT, which contains food and agriculture statistics for more than 245 countries. Years of study for this dataset ranged from 1980-2050.  Consecutive years were 1980-2018 and then 2030 and 2050 years were predicted values. This data was last updated in 2020 and was downloaded in April 2021. 

## Folder structure, file formats, and naming conventions 

Folders within this repository are as follows:

* Code: contains .RMD files with R code from project and one knitted .PDF

* Data: contains processed and raw subfolders with datasets in .csv form. In the raw folder, there are also metadata files associated with the raw data, including Def_Element.csv, Def_Item.csv, FAOSTAT_data_Metadata.csv, and MoreMetadata.pdf. The processed folder contains .csv files from filtering the raw dataset. 

* Output: contains .PNG picture files used in class presentation

* Project: contains a variety of file types used for class presentation and final report. These include .PPT, .RMD, and .DOCs. 


## Metadata

* Raw File (FAOSTAT_data_1980_2050.csv) 

**Column Name** | **Description** | **Class** | **Units**
--------------- | ------------- | ------------- | -------------
Domain Code | Domain number within FAOSTAT for manure management | character | none  
Domain | Domain description within FAOSTAT for manure management | character | none  
Area Code | Code for dataset country | numeric | none  
Area | Name of dataset country | character | none  
Element Code | Code for element | numeric | none  
Element | Name of emission type or stock | character | none  
Item Code | Code for livestock animal | numeric | none
Item | Name of livestock animal | character | none
Year Code | Code of year | numeric | year
Year | Year | numeric | year
Unit | Unit type corresponding to element | character | within itself
Value | Value of unit type of element | numeric | correspond to Unit
Flag | Code corresponding to calculation of value | character | none
Flag Description | Description of how value was calculated | character | none  

* Processed files 
  + CH4_allyears.csv

**Column Name** | **Description** | **Class** | **Units**
--------------- | ------------- | ------------- | -------------
Year | Year from dataset | numeric | year
Mean.Methane | Mean methane emission value from corresponding year | numeric | gigagrams (gg)
Sum.Methane | Total methane emission value from corresponding year | numeric | gg

* Processed files
  + CH4_alltime.csv

**Column Name** | **Description** | **Class** | **Units**
--------------- | --------------- | ------------- | -------------
Element | Name of emission type or stock | character | none
Item | Name of livestock animal | character | none
Year | Year | numeric | year
Unit | Unit type corresponding to element | character | within itself
Value | Value of unit type of element | numeric | correspond to Unit

* Processed files
  + CH4_items.csv

**Column Name** | **Description** | **Class** | **Units**
--------------- | ------------- | ------------- | -------------
Element | Name of emission type or stock | character | none
Year | Year | numeric | year
Unit | Unit type corresponding to element | character | within itself
Asses | Element value corresponding to animal asses | numeric | gg
Cattle,dairy | Element value corresponding to animal dairy cattle | numeric | gg
Cattle, non-dairy | Element value corresponding to animal non-dairy cattle | numeric | gg
Chickens, broilers | Element value corresponding to animal broiler chickens | numeric | gg
Chickens, layers | Element value corresponding to animal layer chickens | numeric | gg
Ducks | Element value corresponding to animal ducks | numeric | gg
Goats | Element value corresponding to animal goats | numeric | gg
Horses | Element value corresponding to animal horses | numeric | gg
Mules | Element value corresponding to animal mules | numeric | gg
Sheep | Element value corresponding to animal sheep | numeric | gg
Swine, breeding | Element value corresponding to animal breeding swine | numeric | gg
Swine, market | Element value corresponding to animal market swine | numeric | gg
Turkeys | Element value corresponding to animal turkeys | numeric | gg


## Scripts and code

The code files can be found in the "Code" folder.  Data_Processing.RMD was where data wrangling and filtering for the project was conducted. Data_Exploration.RMD was where we explored the data visually and numerically. Data_Analysis.RMD was where we conducted our time series analysis and ANOVA test. 


## Quality assurance/quality control

After examining our data, we did not feel that any QA/QC procedures needed to be taken. 


