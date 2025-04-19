# Beyond the Threshold: Customer Insights to Drive Delivery Strategy

This repository contains the full analysis and modeling code for the Swire Coca-Cola Capstone project, created by Imogen Holdsworth and Madalyn Young as part of the University of Utah MSBA program. The focus of this project was to identify Swire’s  emerging customers using various modeling techniques. 

## Business Problem

Swire currently faces a challenge in systematically identifying emerging customers, those who are growing and approaching key volume thresholds, which limites their ability to confidently apply routing strategies that best align with customers ordering behavior. 

Our project provides a predictive framework to support red truck delivery decisions and prevent premature offboarding of potentially high-value customers.

> 📄 See `BPS.pdf` for the full Business Problem Statement.

##  Project Objectives
Identify the emerging customers that are approaching order volume of 400 gallons/cases a year.
Segment customers based on performance and growth potential. 
Support delivery planning with quantitative customer insights. 

## Files and Deliverables

| File | Description |
|------|-------------|
| `Exploratoy_Data_Analysis.Rmd` | Initial EDA |
| `Group2CapstoneModeling.Rmd` | Main modeling pipeline|
| `BPS.pdf` | Official Business Problem Statement|| 
`Capstone SWIRE - Group 2.pdf` | Final presentation slides |

##  Analytics & Modeling Approach

### 1. **Exploratory Data Analysis**
- Investigated order trends, outliers, seasonal patterns, and customer geography.
- Key insights include high variation in baseline volume and YOY growth by customer type, distinct customer locational segments, retail and non retailer customer differences, and customer segmentation based on ordering trends

### 2. **Customer Segmentation**
Customers were grouped based on:
2024 order volume and year over year growth rates. 
Customers were assigned into one of the 6 segments:
Low Volume High Growth, Low Volume Low Growth, High Volume High Growth, High Volume Low Growth, Transitory Growing and Transitory Declining.
Retailer or non retailer customer status

### 3. **Modeling Framework**
In order to support delivery insights for all customers, two routes of analysis were completed, one for the retailer customers and one for the non retail customers. 

- **Non-Retail Customers**:
  - Used multilevel logistic models (MLM) to predict 2024 order volumes.
  - Incorporated random effects for customer segments to capture unobserved group behavior.

- **Retail Customers**:
  - Included group-level predictors like outlet count and group performance.
  - Modeled using mixed-effects models to account for nested structures of customers within a retailer.

##  Key Results
563 customers identified to be approaching key volume thresholds (not currently at threshold, but approaching threshold) 
Developed a segmentation informed delivery strategy, which would support tailored strategies for each customer ( ARTM, Direct delivery) 

## Future Recommendations

- Integrate additional historical ordering data to calculate a compounded annual growth rate.
- Leverage additional financial insights such as profit and loss to refine routing decisions.
- Consider expanding on the model to develop further insights into the reliable (High volume) customers. 


## Authors
**Madalyn Young** and **Imogen Holdsworth**
