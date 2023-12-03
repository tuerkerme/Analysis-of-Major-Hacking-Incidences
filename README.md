# Analysis-of-Major-Hacking-Incidences
## Table of Contents
 - [Project Overview](#Project-Overview)
 - [Data Source](#Data-Source)
 - [Tools](#Tools)
 - [Data Cleaning/Preparation](#Data-Cleaning/Preparation)
 - [Exploratory Data Analysis](#Exploratory-Data-Analysis)
 - [Findings](#Findings)
 - [Recommendations](#Recommendations)
 - [Limitations](#Limitations)
   
## Project Overview

This data analysis project covering the years 2004 to 2022 aims to provide insights into cyber attacks on the significant entities targeted, hacking methods employed, and the diverse range of organization types impacted. 
<img width="556" alt="image" src="https://github.com/tuerkerme/Analysis-of-Major-Hacking-Incidences/assets/149696414/7d1eeec4-0efb-4d8e-bf2a-bac2b74eade6">

 
## Data Source
Cyber Security Data: The primary dataset used for this analysis is the "df.csv" file obtained from Kaggle.com, containing detailed information about hacked companies, their sectors and attack type. 
 
## Tools
```
Python: Data Cleaning
Excel: Data Cleaning
Tableau: Data Visualization
 ```
## Data Cleaning/Preparation

In the preliminary stages of data analysis, meticulous attention was given to the following key tasks within the data preparation phase:
```
Data Loading and Inspection:
Thorough examination and loading of the dataset to gain a comprehensive understanding of its structure, variables, and overall quality.

Handling Missing Values:
Implementation of rigorous strategies for managing and mitigating the impact of missing data, ensuring completeness and reliability.

Data Cleaning and Formatting:
Rigorous data cleaning procedures were executed to rectify inaccuracies and inconsistencies, followed by meticulous formatting to uphold data integrity.
```
These steps were integral in refining the dataset to a state conducive to subsequent analytical endeavors.

This stage included some interesting code/features worked with
 
 ```
 df=pd.read_csv("df_1.csv")
 df.head()
 df.info()
 df.shape
 df.describe()
 df.isnull().sum()
 df.dropna(inplace=True)
 df.duplicated().sum()
 df.to_excel('Cyber_attacks.xlsx', index=False)
 ```


## Exploratory Data Analysis
EDA involved exploring the cyber attack data to answer key questions, such as:
 ```
In which years did the cyber attacks occur most frequently?
Which sectors have experienced the greatest impact from these cyber attacks?
What are the prevailing attack types observed in these incidents?
 ```
## Findings
 
The analysis results are summarized as follows:
 
The analysis indicates that companies in the web, health, and financial sectors are most affected by cyber attacks. The number of attacks increased in 2011, 2019, and 2020, with a sharp decline in 2021 and 2022. The most common types of attacks are attributed to poor security measures, incidents involving lost or stolen media, and unintentionally published credentials.

Product Category A is the best-performing category in terms of sales and revenue.
Customer segments with high lifetime value (LTV) should be targeted for marketing efforts.

## Recommendations

Given the findings of the analysis, we would recommend implementing robust security measures tailored to address the specific vulnerabilities observed in the web, health, and financial sectors. Focus should be placed on enhancing security protocols to mitigate the risks associated with poor security practices, securing sensitive data to prevent loss or theft of media, and implementing stringent controls to avoid accidental disclosure of credentials.

Additionally, investing in up-to-date cybersecurity technologies, conducting regular security audits, and providing comprehensive training for employees to raise awareness about potential threats could significantly contribute to bolstering the overall cybersecurity posture. Continuous monitoring and adaptation of security strategies in response to emerging threats are also crucial to staying ahead of the dynamic landscape of cyber risks.

Moreover, collaboration with industry peers, information sharing forums, and staying informed about the latest cybersecurity trends and best practices would contribute to a proactive and resilient cybersecurity approach. By addressing these recommendations, organizations can better safeguard their critical assets and effectively navigate the evolving cybersecurity landscape.


## Limitations

I had to remove all null values because they would have affected the accuracy of my conclusions from the analysis.
