# HR-PERFORMANCE-APPRAISAL

## Table of Content

- [Project Overview](#project-overview)
- [Data Sources](#data-sources)
- [Tools](#tools)
- [Data Cleaning](#data-cleaning)
- [Recommendations](#recommendations)
- [Exploratory Data Analysis](#exploratory-data-analysis)
- [Data Analysis](#data-analysis)
- [Results](#results)
- [Recommendations](#recommendations)
- [Limitations](#limitations)
- [Reference](#reference)

### Project Overview

This data analysis, tracks and monitors Employee's Development, performance  with real-time insight of the HR department of a company over the past the year. By analysing various aspects of the data, we seek to identify trends, and make a data driven decisions and recomendation, and by doing this we gain a proper and a deeper understanding of the company's employee deveolopment and performance.

![Dashboard](https://github.com/user-attachments/assets/602dfa20-da0f-477d-b030-3ab0ca5107ca)


### Data Sources

Sales Data: The promary dataset used for this analysis is the "Cleaned_HR_Data_Analysis Part 1.csv" and "2nd part of the HR Dataset.csv" files, These files contains detailed information about employees of the company.

### Tools

- Excel - Data Cleaning
- PowerBI - Creating Reports and Data Visualization



  ### Data Cleaning

  In the initial data preparation phase, we performed the following tasks:
  1. Data loading and inspection.
  2. Handling missing values.
  3. Handling duplicates values and entries.
  4. Data cleaning and formatting.

### Exploratory Data Analysis

EDA invlvolved exploring the HR datasets to asnwer key questions, such as:

- Turnover/Attrition rate?
- Average training cost per employee?
- Diversity Ratio?
- Performance Score Distribution?
- Average Tenure by Department?
- Training Participation Rate?
- Engagement-Satisfaction Correlation?


  ### Data Analysis
  This includes some interesting code/features worked with

   ```Powerbi
Role Status = SWITCH( TRUE(), Cleaned_HR_Data_Analysis[Title] ="Area Sales Manager" , "Leadership",
Cleaned_HR_Data_Analysis[Title] = "Director of Operations", "Leadership", 
Cleaned_HR_Data_Analysis[Title] = "Director of Sales", "Leadership",
Cleaned_HR_Data_Analysis[Title] = "IT Director", "Leadership",
Cleaned_HR_Data_Analysis[Title] = "IT Manager -DB", "Leadership", 
Cleaned_HR_Data_Analysis[Title] = "IT Manager - Infra", "Leadership",
Cleaned_HR_Data_Analysis[Title] = "IT Manager - Support", "Leadership", 
Cleaned_HR_Data_Analysis[Title] = "President & CEO", "Leadership",
Cleaned_HR_Data_Analysis[Title] = "Production Manager", "Leadership",
Cleaned_HR_Data_Analysis[Title] = "Sales Manager", "Leadership",
Cleaned_HR_Data_Analysis[Title] = "Senior BI Manager", "Leadership",
Cleaned_HR_Data_Analysis[Title] = "Shared Service Manager", "Leadership",
Cleaned_HR_Data_Analysis[Title] = "Software Engineering Manager", "Leadership",
Cleaned_HR_Data_Analysis[Title] = "Sr. Accountant", "Leadership",
Cleaned_HR_Data_Analysis[Title] = "Sr. Network Manager", "Leadership","Non Leadership") ;



### Results

1. Non leadership department has the lowest attrition rate which is 48.37 percent, Leadership department such as the executive office and admin offices  has the highest attrition rate which is 48.71 percent.
2. The performance distribution rating is very low with the “Need Improvement” rate at 58.63 percent and “exceed expectation” at  41.3 percent.
3. The rate at which employee leaves the software engineering department before 1 year tenure at the office is very high.

### Recommendations

- With the high attrition rate at the leadership role a further exploratory data analysis can be done to check if the quality of training being offered to staffs at the leadership role has an impact on the attrition level of the organization.
- With the organization training success rate at 51 percent, this can be worked on and improvement can be made by ensuring more staff completes their training.

### Limitations
I had to format all currency column with currency signs and working with two split datas was a bit tricky, this would have affected the outcome and accuracy  of my analysis. but even at that we were able to see that there is a positive correlation between the engagement score and Satisfaction scores.


### Reference

1. 10 10 10 10 written by Chandoo
2. [Datacamp](https://campus.datacamp.com/pdf/web/viewer.html?file=https://projector-video-pdf-converter.datacamp.com/33412/chapter4.pdf#page=16)



