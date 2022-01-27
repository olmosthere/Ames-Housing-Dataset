# Project 2 - Ames Housing Data and Kaggle Challenge


## Problem Statement

You have been contracted by Ames Remodeling Contractors (ARC) Inc. to help them assess whether they can gain a competetive advantage by helping their prospective clients estimate how much a particular remodeling project can increase their property value.  

## Data Dictionary

You can access a copy of the data dictionary here: http://jse.amstat.org/v19n3/decock/DataDocumentation.txt

## The Data Science Process

Created a linear regression model to help ARC predict property values based on features of the property.

### Data Cleaning and EDA

- Cleaned data of null values, either replacing them with 'NA', 0, or droping the rows from the training data.
- Viewed distributions to identify skewed data fields.
- Removed outliers 3 standard deviations above or below the mean for Sale Price and Lot Size for training data.
- Created Heat Map to highlight which features should be included in our features matrix.
- Created pairplot to visualize linear relationships between features and target.
- Provided summary statistics

### Preprocessing and Modeling

- Created dummy columns for all catagorical data that resulted in a higher adjusted R2 upon its inclusion.
- Designed an iterative loop that allows users to specify X values, instantiate a linear regression model, fit it to the
training data, test the model's performance based on RMSE, R2, and Adjusted R2, and add it to a dataframe that compiles 
the results of multiple iterations.

### Conclusion and Recommendations
- Adding fireplaces, garages, pools, and any amount of living space would increase property value.
- However, doing these project for the sole sake of increasing property value is not advisable.
- Focus on utilitarian projects and frame any increase in property value as a discount.
- Unless it’s a major remodel, our model currently isn’t accurate enough to predict small changes in property value since
our RMSE is still high and small increases will most likely be lost in the margin of error.
