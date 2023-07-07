
![image](https://github.com/DennisWainaina/Phase_2_final_project/assets/116555573/27b2e879-a805-4d51-a294-7fb46e1a538a)

## PHASE 2 FINAL PROJECT

## 1. INTRODUCTION
**Welcome to my GitHub repository for the Megamax Real Estate Agency project!** 

In this project, we aim to analyze how home renovations can impact the sale prices of houses. Megamax Real Estate Agency, a prominent agency in New York, has initiated a new division that connects home sellers with potential buyers. To assist their clients in making informed decisions and increasing the market appeal of their properties, they want to understand the effects of renovations on sale prices.

As a Data Scientist, I was hired by Megamax Real Estate Agency to predict the impact of renovations on house prices. Through comprehensive analysis and modeling, I will present my findings and insights to the head of the new division. These insights will enable the division to advise potential sellers effectively and provide guidance on how renovations can influence the sale price of their homes.

This README.md document provides an overview of the project and its main segments:
1. [OBJECTIVES](#Objectives)
2. [BUSINESS UNDERSTANDING](#business-understanding)
3. [DATA UNDERSTANDING](#data-understanding)
4. [DATA PREPARATION](#data-preparation)
5. [EXPLORATORY DATA ANALYSIS](#exploratory-data-analysis)
6. [MODELLING](#modelling)
7. [CONCLUSION](#conclusion)
8. [RECOMMENDATIONS](#recommendations)

Thank you for visiting my GitHub repository for the Megamax Real Estate Agency project. Let's dive into the analysis and explore the relationship between home renovations and sale prices!

## OBJECTIVES
The objectives of the project are:
- To determine how rennovations affect the saleprice of the home of a potential sellor.
- To present findings and model to head of division so that the head may use the insights generated to advise potential sellors(clients).

## BUSINESS UNDERSTANDING
#### 3.1 PROBLEM STATEMENT
To determine the effect of home rennovations on the saleprice of a home. This is to help Megamax Real Estate Agency in making informed decisions to potential sellors of homes who are their clients.

#### 3.2 MEASUREMENT OF SUCCESS
The goal is to determine the effect of home rennovations on the saleprice of homes. The measure of success will therefore be after analysis has been done and insights generated,findings should be presented to the head of the new divisions who will use both to advise new sellors appropiately.

## DATA UNDERSTANDING
For the problem at hand the data used to see the effect of rennovations on the price of houses was the King County House Sales dataset. This dataset was sourced from Kaggle and is relevant to the problem at hand as it contains data about relevant features of houses together with the price of such homes. These features are in the form of columns in a dataframe and they include:

- **Price** : This is the target(dependent) variable and is what we want to see the effect of rennovations on.

- **Bedrooms**: This is the number of bedrooms a house has and is one of the rennovations that may be performed to see the effect of SalePrice such that one may add or remove bedrooms to see the effect on SalePrice.

- **Floors**: This is the number of floors a house has and is relevant to the problem as a potential sellor may want to know the effect of adding or removing floors may have on the selling price of his/her home.

- **Condition**: This is the overall condition which has unique values as follows ['Average', 'Very Good', 'Good', 'Poor', 'Fair']. It is relevant to our problem as the client may want to know whether rennovation of the house to make it look new will increase or decrease the selling price of the house.

- **sqft_above**: This is the overall square footage of the house minus the basement. It is relevant as this factor shows whether the size of the house minus the basement determines its selling price. A client with enough land may even decide to increase its size to see if it will increase its asking price.

- **waterfront**: This is the prescence of a waterfront in front of the house. A client may want to know whether adding a waterfront will decrease or increase the selling price of his/her home.

- **grade**: This is the type and quality of the material used in construction of houses. It also includes the finishing and the design quality of the house and the interiors. It is relevant to the problem as a client may want to know whether using high quality materials in the rennovation of his/ her house will lead to increase or decrease in the price of the house.

## DATA PREPARATION

Before data is used for analysis one must ensure the data is clean. This is by:

- **Removing outliers**: Identification and removal of data points that deviate significantly from the overall distribution, as they can adversely impact analysis results.

- **Handling missing values**: Thoroughly checking for missing values and employing appropriate strategies to handle them, such as imputation techniques or assessing the suitability of the missing data for analysis.

- **Identifying and resolving duplicates**: Identifying and removing duplicate records to ensure data integrity and avoid bias in analysis outcomes.

- **Assessing columns with excessive missing values**: Evaluating columns with a substantial number of missing values and determining their relevance to the analysis. Dropping columns that are not essential or exploring alternative strategies for handling missing data.


- **Correcting data types**: Verifying and correcting the data types of variables to align them with their intended representation (e.g., converting numerical data from strings to numeric types).


## EXPLORATORY DATA ANALYSIS
Here is a summary of the analysis from EDA.

#### UNIVARIATE ANALYSIS
Univariate analysis involves examining individual variables in isolation to gain insights into their distribution, central tendency, and dispersion. In this project, we performed univariate analysis on the dataset to understand the characteristics and patterns of the variables. Here are the key findings:

1.**Distribution of Numeric Variables**: We visualized the distribution of numeric variables such as price, square footage, number of bedrooms, bathrooms, and floors using histograms and box plots. Most variables followed a roughly normal distribution, indicating that the data was relatively symmetrical. Outliers were identified, and appropriate measures were taken to handle them.
![image](https://github.com/DennisWainaina/Phase_2_final_project/assets/116555573/73f8168a-4c49-4386-8ee4-6a53d52186c4)

Here we also wanted to see how far the values were distributed from the mean which as shown below from the boxplot was not much.
![image](https://github.com/DennisWainaina/Phase_2_final_project/assets/116555573/906997fb-238b-4301-a1aa-811942e90581)


2.**Categorical Variables**: We examined categorical variables such as grade, condition, view, and waterfront. These variables were converted into numeric representations to assess their relationship with the dependent variable (price). We plotted bar charts to visualize the mean price for each category. It was observed that certain categories, such as higher grades, better conditions, and improved views, were associated with higher average sale prices.
![image](https://github.com/DennisWainaina/Phase_2_final_project/assets/116555573/881878ea-74c2-444d-8e45-aa5a33eb56de)
![image](https://github.com/DennisWainaina/Phase_2_final_project/assets/116555573/23e00777-7c9b-4fb2-a20d-eece958c6a92)
![image](https://github.com/DennisWainaina/Phase_2_final_project/assets/116555573/88def7ed-5216-4502-87a0-27d5167afd92)

#### BIVARIATE ANALYSIS
Here we wanted to see how the independent variables were correlated with each other and the dependent variable price. This is summarised in the two pictures below.
![image](https://github.com/DennisWainaina/Phase_2_final_project/assets/116555573/59a8777b-27ed-4136-806b-bcf7ea55a034)
**Correlation matrix of the variables using a heatmap.**
![image](https://github.com/DennisWainaina/Phase_2_final_project/assets/116555573/c0154bdc-ab23-4024-96db-6ca6a5adaffc)
**Scatterplot of all the independent variables against the dependent variable.**

## MODELLING
Here is the summary findings of our model:
- It is interesting to note that for the multiple linear regression model the values which had the highest gradient are the categorical variables turned numeric.

- The slopes for grade, waterfront, condition and view had slopes of **7.528e+04, 2.481e+05, 2.813e+04, 3.427e+04** respectively with **waterfront** being the highest.

- This indicates that the grade of the house, the prescence of a waterfront, the condition of the house and the quality of the view had the highest effect on the selling price of the house.

- An increase in sqft_living and the number of bathrooms also seemed to increase the selling price of the house.

- Potential sellors looking to increase the price of their houses should therefore look to improve the grade of their houses, add a waterfront, improve the condition of the house and improve the quality of the view.

- They should also look to increase the number of bathrooms and the sqft_living of their homes.

## CONCLUSION
In conclusion, we have successfully analyzed the relationship between home renovations and sale prices using the King County House Sales dataset. Our findings highlight the importance of considering factors such as grade, size, condition, and specific amenities when aiming to maximize the selling price of a house. The insights generated from this analysis will enable Megamax Real Estate Agency to provide informed advice to their clients, empowering them to make decisions that enhance the market appeal and value of their homes.

## RECOMMENDATIONS
1.**Focus on Improving Grade and Quality**: The grade of a house and the quality of its construction materials and finishes have a significant impact on the sale price. Therefore, clients should consider using high-quality materials and investing in upgrades that enhance the overall grade of their homes. This can include: improving the design, interiors, and construction elements to attract potential buyers and command a higher selling price.

2.**Enhance Living Space**: The size of the living space, as indicated by variables like sqft_living and bedrooms, strongly correlates with the sale price. Clients should explore opportunities to increase the living area by adding rooms or expanding existing spaces. This can significantly impact the perceived value of the property and potentially lead to higher offers from buyers.

3.**Consider Floor Upgrades**: The number of floors in a house also influences the sale price. Clients should evaluate whether adding or removing floors is feasible and financially viable for their properties. Additional floors can offer more living space and potentially increase the sale price, especially if the local market demands multi-story homes.

4.**Pay Attention to Property Condition**: The overall condition of the house plays a role in determining its value. Clients should focus on maintaining their homes in good condition and consider renovations or repairs that improve the condition rating. Updating features like the roof, HVAC systems, and interior finishes can positively impact the sale price and attract buyers looking for well-maintained properties.

5.**Assess Waterfront Opportunities**: Waterfront properties can have a desirable appeal and command higher sale prices. Clients who have access to waterfront locations should consider highlighting this feature and incorporating it into the marketing strategy. Enhancements such as landscaping, outdoor amenities, or creating direct access to the waterfront can further enhance the property's value.

6.**Seek Professional Guidance**: It is advisable for clients to consult with professionals in the real estate industry, such as real estate agents or property appraisers, who have expertise in local market conditions. These professionals can provide valuable insights and guidance specific to the area, helping clients make informed decisions regarding renovations and pricing strategies.

### Overall, by implementing these recommendations and considering the specific characteristics of their properties, clients can optimize the sale price of their homes and increase market appeal. It is crucial for clients to carefully evaluate the costs and potential return on investment for each renovation or improvement before proceeding.




