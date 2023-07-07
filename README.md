## PHASE 2 FINAL PROJECT
![image](https://github.com/DennisWainaina/Phase_2_final_project/assets/116555573/27b2e879-a805-4d51-a294-7fb46e1a538a)

## 1. INTRODUCTION
**Welcome to my GitHub repository for the Megamax Real Estate Agency project!** 

In this project, we aim to analyze how home renovations can impact the sale prices of houses. Megamax Real Estate Agency, a prominent agency in New York, has initiated a new division that connects home sellers with potential buyers. To assist their clients in making informed decisions and increasing the market appeal of their properties, they want to understand the effects of renovations on sale prices.

As a Data Scientist, I was hired by Megamax Real Estate Agency to predict the impact of renovations on house prices. Through comprehensive analysis and modeling, I will present my findings and insights to the head of the new division. These insights will enable the division to advise potential sellers effectively and provide guidance on how renovations can influence the sale price of their homes.

This README.md document provides an overview of the project and its main segments:
1. [OBJECTIVES](#Objectives)
2. [BUSINESS UNDERSTANDING](#business-understanding)
3. [DATA UNDERSTANDING](#data-understanding)
4. [DATA PREPARATION](#data-preparation)

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
