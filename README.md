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
The sales for the tick vaccine between the different regions of Australia varied significantly which is revealed in the barplot. The barplot was cutomised to better visdualise the result. The las argument allows to change the orientation of the axis labels to vertical. The axis size was also customised using the cex.names argument. 


### Investigation of the sales for the Tick Fever Vaccine in the frozen and chilled forms 
A data frame was first created to record the calculated percentages of frozen and chilled tick vaccine sales. The data was then visdulised using a barplot with the function of ggplot. Following by the bar graph, a pie chart was created using the polar coordinates argument as an extension of the bar graph to better illutrate the sales of the vaccine in two different forms. 

## Key findings
1. The sales for the tick vaccine between the different regions of Australia varied significantly which is revealed in the barplot. It’s found that Central, QLD has the highest amount of sales for the tick vaccine. The sales in this region of Australia has over 100,000 more sales than other regions. When looking at the other regions, we found that only Brisbane, Wide Bay and North Wes have some noticeable sales of the tick vaccine, and that the rest have very low or zero sales of tick vaccine. This is probably due to the fact that Queensland is the largest supplier of beef for Australia, hence due to their large amount of cattle the vaccine is in high demand to prevent the tick fever from causing detrimental impacts. However the state of NSW is the second biggest supplying state for beef and hence the sales should be at a higher amount. The low sales from other regions could be due to the people’s misunderstanding and the lack of knowledge about tick vaccine. Some people question the protection and usefulness of the vaccine, as well as its duration. The sales of tick vaccine may also be affected by the endemicity of Babesia bovis,Babesia bigemina and Anaplasma marginale. Without the spread of the tick fever, the lifestocks won’t need the vaccination. The benefits of the vaccination definitely exceeds its risk, however according to the dataset, there is still a lot that should be done by the Government to promote the acceptance of the vaccine.

2. According to the calculated percentages and the pie chart, the chilled tick fever vaccine has a significantly higher amount of sales than the frozen vaccine. Altogether, there was 300095 chilled vaccines sold compared to 18975 frozen vaccines. Despite the frozen vaccine to have a much higher shelf life of approximately 5 years, compared to the chilled vaccines of 4 days, the chilled vaccine is of higher popularity. This would be due to the reason that those who buy the tick vaccine would be vaccinating the cattle immediately, as they might be in desperate need of the vaccine. Also the immedient use of the vaccine limits potential risks such as causing the vaccine to become ineffective due to incorrect storage conditions and other implications. However the small percentages of frozen vaccines that are bought would be sold to those who live in rural areas that would need a vaccine with longer shelf life, as well as the vaccines that could be delivered overseas. Farmers in these circumstances are not able to have the vaccine delivered within its shelf life therefore can only use the frozen vaccine. Also, larger businesses might prefer to have the vaccine on hand for their convenience and hence take advantage of the large shelf life of the frozen vaccine. Hence this research question enables increased understanding about the sale market for tick vaccine in Australia.
