# MATH1005
## Introduction 
This project aims to investigate the vaccination rate of Tick Fever vaccine acorss different states in Australia. Using the data obtained from the Agriculture and Fisheries of Queensland Government, we were able to conduct data profiling, mining and analysis using R studio. The research discovered that central Queensland had the highest amount of tick vaccine sales compared to any other state in Australia. On the other hand, frozen vaccines were a lot more popular than chilled vaccines due to the fact that they had a lot longer shelf life. This report provides ingihts for the Australian government to reallocate its production of the Tick Fever vaccine based on the market demand. It also provides insights for the government to improve the vaccination rate in Australia in order to prevent the spread of tick fever. 
### Resulting graphs 
#### Graph 1. The sales of tick fever vaccine across the states in Australia
<img width="619" alt="截圖 2022-11-20 下午1 42 56" src="https://user-images.githubusercontent.com/117743186/202887521-924231bf-0a8f-4739-b619-ea5d5dae80b0.png">

#### Graph 2. The sales of the tick fever vaccines in the frozen and chilled forms
<img width="620" alt="截圖 2022-11-20 下午1 44 22" src="https://user-images.githubusercontent.com/117743186/202887542-6ace655e-37b9-4041-80b0-75e8eb51b208.png">

## Features
- Data retreival 
- Data preparasion was completed using R. The following investigations were conducted:
  - Data cleansing: The null variles were eliminated from the dataset
  - Data merging 
  - Classification of variables
- Investigation of the vaccination rates across the states in Australia
- Investigation of the sales for the Tick Fever Vaccine in the frozen and chilled forms 

## Content
### Data Retrieval 
The data of the Tick Fever Vaccine sales was provided by Queensland Governemnt on the Open Data Portal. This dataset records the amount of tick vaccines sold for beef cattle in Australia between 1/7/13-30/9/13 in two forms; chilled trivalent (3 germ) vaccine and frozen trivalent vaccine (marketed as Combavac 3 in 1). The dataswet can be downloaded on: http://www.daff.qld.gov.au/__data/assets/file/0007/99754/tick-fever-vaccine-sales-jul-sep-13.csv 

### Data Dictionary
| **Column** | **Type** |
| :-------------: | :-------------: |
| Territory  | text  |
| Chilled  | numeric  |
| Frozen  | numeric  |
| Total  | numeric  |

### Data preparasion 
After retreival of the dataset, data cleaning was conducted to eliminate the null and zero values. In order to understand the data set, classification of the variables were conducted. Within the three variables identified from the dataset, two of them were qualitative varibles while the other one was quantitative varible for sales. Lastly, data wanrlging was completed to merge the cells with the same regions into one. Therefore, the region column changed from 26 to 13 variables. One extra column was added for the sums of the vaccine sales in each region as well. This column is used for later processing.

### Investigation of the Tick Fever vaccination rates across the states in Australia


### Investigation of the sales for the Tick Fever Vaccine in the frozen and chilled forms 
A data frame was first created to record the calculated percentages of frozen and chilled tick vaccine sales. The data was then visdulised using a barplot with the function of ggplot. After all, a pie char was creating as an extension of the bar graph to even better illutrate the sales of the vaccine in two different forms. 
