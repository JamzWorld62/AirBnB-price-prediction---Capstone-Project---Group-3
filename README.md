# Airbnb Listing Price Prediction

## Project Overview
This project aims to develop a machine learning-based solution to suggest appropriate listing prices for Airbnb properties in Antwerp, Belgium. By analyzing historical data and identifying key factors influencing prices, we build a predictive model to help hosts optimize their pricing strategies and maximize revenue.

## Data
The dataset used in this project is sourced from Airbnb and consists of the following tables:
- Calendar: Listing availability and price information over time
- Listings: Details of each listing, including property type, room type, and amenities
- Hosts: Information about the hosts of the listings
- Reviews: Guest reviews for the listings

The data is preprocessed and aggregated to create a unified dataset for analysis and modeling.

## Methodology
The project follows these main steps:

1. Data Understanding and Feature Creation:
   - Examine the Calendar and Listings tables
   - Clean and preprocess the data
   - Create relevant features through data aggregation

2. Data Quality and Checks:
   - Check for missing values and handle them appropriately
   - Analyze descriptive statistics for numeric variables
   - Examine frequency counts for categorical variables

3. Variable Profiling and Relationships:
   - Compute correlation matrix to identify variable relationships
   - Visualize relationships using scatter plots and box plots
   - Drop variables with low correlation to the target

4. Modeling and Evaluation:
   - Split the data into train, validation, and test sets
   - Experiment with different regression models (Linear Regression, Decision Tree, Random Forest, Gradient Boosting)
   - Evaluate models using RMSE and R-squared metrics
   - Select the best-performing model (Random Forest) based on validation metrics
   - Evaluate the selected model on the test set

5. Insights and Recommendations:
   - Identify key factors influencing listing prices
   - Provide actionable recommendations for Airbnb hosts to optimize pricing
   - Discuss potential improvements and future work

## Results
- The Random Forest model achieved the best performance on the validation set, with an RMSE of 55.39 and an R-squared of 0.07.
- The top 5 important predictors of listing prices are:
  1. Property type (Entire villa)
  2. Listing ID
  3. Number of bedrooms
  4. Number of bookings
  5. Number of beds
- Hosts can leverage these insights to set competitive prices based on their property characteristics and booking trends.

## Usage
To reproduce the analysis and run the code:
1. Clone this repository: `git clone https://github.com/[your-username]/airbnb-price-prediction.git`
2. Install the required dependencies: `pip install -r requirements.txt`
3. Run the Jupyter notebooks in the following order:
   - `data_preprocessing.ipynb`: Preprocess and aggregate the data
   - `exploratory_data_analysis.ipynb`: Perform exploratory data analysis and variable profiling
   - `modeling.ipynb`: Train and evaluate different regression models
4. Modify the notebooks as needed and experiment with different techniques and parameters.

## Dependencies
- Python 3.7+
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

Please refer to the `requirements.txt` file for the complete list of dependencies.
