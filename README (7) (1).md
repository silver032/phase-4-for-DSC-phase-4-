### Overview

This project uses sales data from an E-commerce website, the goal of the project is to determine ideal inventory level (itemcount). There are several irrelevant features in the dataset (such as SKU_number). The features being used are sold count, sold flag, strength factor and others. Overall the dataset wasn't ideal due to its shape, outliers, and binaries. 

# Dataset Description

The dataset includes several variables regarding marketing channel, sold count, sold flag, new release flag, strength factor, and release year. Strength factor couldn't be determined based off the research done on the dataset from Kaeggle. 

# Business Problem 

The project is commissioned by E-COMMERCE Global to determine ideal inventory levels for stock. 

- What impact will it have if we can predict ideal inventory levels?
- What are some historical trends for items and how does it impact inventory?
- What other efficencies?

# Goals

Predictive Analysis: To predict through regression how much of each item should be kept in stock. 
Indicator Analysis: To identify what features impact sales of items. 

# Key Questions

1. What preprocessing steps do we need to take to create an effective predictive model?
2. Which type of predictive model gets the best results?
3. What hypertuning techniques are used to tune the model?
4. What are the benefits of our model?

# Target Variable Investigation

Target variable is Itemcount; How many items do we need? What features impact this number?


# Preprocessing Steps

# Data Cleaning: 
 Handling missing values and removing irrelevant features. Converting Release year to age. Converting lowuserprice (price sold at) and price reg (listed price) to price difference. 

# Data Scaling and inputing: 
Applying appropriate techniques to handle numerical variables, inputer and scaler

## Predictive Modeling

# Model Selection: 
Evualted 8 different models to 

# Model Comparison:
We focused on R^2 as our performance metric and compared R^2 of each. 

# Hyperparameter Tuning
Fine-tuned using RandomizedGridsearch techniques to optimize performance, focused on improving R^2 to improve model accuracy. 

## Exploratory Data Analysis 

# Overall Datashape 



Large number of binaries


# Heatmap vs target

for item sold, shows high frequency outliers

# Feature correlation matrix

Shows low correlation between features and targets

## Model results 

After running various models, our R^2 shows that randomforest and catboost had the best results. 


- Ran 8 different models for multicolinarity 

# Hypertuned Model Results


Both models improved slightly, indiciating undersampling. With more time can run more robust hypertuning. 

# Feature importance for random forest

Shows that Strength Factor and price have biggest impact on item count.



# Recommendations

- For an inventory management system, having an R^2 around 0.50 suggests that while the model has some predictive power, it might not be sufficient for making reliable inventory decisions.
- Creating a threshold to cut items that aren’t being sold
- Running pilot studies on active inventory 


# Next Steps

- Finding additional datasets
- Utilizing a classifier approach, determining stock or not
- Handling the preprocessing differently 
- Using cross validation, ensemble methods, different sampling techniques to improve the model 


