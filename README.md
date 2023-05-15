# Homelessness
This project uses the data science methodology to investigate homelessness in the U.S.

1. Introduction: 

  The 2020 [point-in-time count](https://www.kingcounty.gov/elected/executive/constantine/news/release/2020/July/01-homeless-count.aspx) of people experiencing homelessness for Seattle/King County was 11,751. This represents a 5% increase over the 2019 count and reflects similar trend across many counties in the western U.S.. 
  
  The U.S. Department of Housing and Urban Development (HUD) produced a report in 2019 [Market Predictors of Homelessness](https://www.huduser.gov/portal/sites/default/files/pdf/Market-Predictors-of-Homelessness.pdf) that describes a model-based approach to understanding of the relationship between local housing market factors and homelessness. 
  
  This project investigates whether there are alternative modeling approaches that outperform the models described in the HUD report.

2. Data: 
  
  The [data](https://github.com/brian-fischer/DATA-3320/blob/main/homelessness/05b_analysis_file_update.csv) for this project are described in HUD's report [Market Predictors of Homelessness](https://www.huduser.gov/portal/sites/default/files/pdf/Market-Predictors-of-Homelessness.pdf) in the section titled DATA.

  The data dictionary [HUD TO3 - 05b Analysis File - Data Dictionary.csv](https://github.com/brian-fischer/DATA-3320/blob/main/homelessness/HUD%20TO3%20-%2005b%20Analysis%20File%20-%20Data%20-%20Dictionary.csv) contains descriptions of all variables in the data set.

3. Date Preparation:

The dataset has 332 distinct variables, which makes it difficult to understand and analyze the data properly. To facilitate the analysis, it is essential to utilize a dictionary to identify the unique values associated with each domain. Since the objective of this project is to predict the prevalence of homelessness, it is important to exclude rows with missing values in this particular category. Furthermore, as the variables "percentage_excessive_drinking" and "migration_4_year_change" only contain data from 2017, the focus of the analysis will be on that specific year. To facilitate further analysis, three new variables,  "rate_homeless," "rate_sheltered," and "rate_unsheltered," are created within the data frame .Additionally, it should be noted that the demographic variables such as race, gender, and age are provided as total counts, which will be converted into percentages for enhanced understanding and analysis.
