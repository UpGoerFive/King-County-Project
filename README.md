# Predicting Sale Prices for Lake and Company Realty
Contributing Members: Abass Ibrahim, Nathaniel Martin, and Matthew Samson
![image](https://github.com/UpGoerFive/King-County-Project/raw/master/images/wonderlane-GBHhIyWftHs-unsplash-cropped.jpg)

## Project of overview
This aim of this project is to utilize linear regression techiques to predict final house sale prices in King County in Washington State. This includes major cities such as Seattle and Redmond. The project is from the perspective of being hypothetically commissioned by Lake and Company Realty in Seattle to produce a model to accurately predict sale prices. Lake and Company will then use these results to more judiciously consider what clients it takes on as well as to appropriately set fees, rates, commissions, and the like. We've produced both a predictive and inferential model for this purpose and we have a few recommendations for Lake and Company based on these models.


## Data
- We utilized a dataset from the King County Assessor's public website, which lists house sale prices and other data for over 21,000 houses in the period from May 2014 - May 2015. 

- We also manually scraped data from UnitedStatesZipCodes.org for a number of additional datapoints and features.

## Methods
Before we did anything else, we performed a train-test split to hold a portion of the data for later scoring after we were satisfied with the performance of our models. After performing exploratory data analysis with visualizations to get a better intuitive understanding of the data, we built a number of predictive models using multiple linear regression. We used K-fold cross validation to score our models as we went. We engineered several features such as distance to the city centers of Seattle and Redmond, among others. Additionally, we created an inferential model to assess the most important feature relationships to price. 

## Results
We produced nearly a dozen predictive models with varying ability to predict final sale price. 

![image](https://github.com/UpGoerFive/King-County-Project/raw/master/images/the_skylar_slide_phase2.png)

- We began with a simple linear regression comparing only price and living space in square feet. This model was only able to account for 49% of the variance in the data with an average error of $249,000. We attempted a number of techniques to improve and refine our models. 

- Ultimately, after incorporating all of our features (including several new engineered features as well as several from our scraped data) with no dummy variables. This model is able to account for 82% of the test data variance with an average error of $160,000, a significant improvement over our initial model. Additionally, the accuracy of our model improves a decent amount for those houses which our model predicts at $1million or less. 
![image](https://github.com/UpGoerFive/King-County-Project/raw/master/images/final_model_graph.png)

In addition to our predictive models, we examined a number of other factors important to price, both through visual data analysis and an inferiential model. For instance, we were interested in the geographic locations of the most expensive houses and produced a map showing price by location.

![image](https://github.com/UpGoerFive/King-County-Project/raw/master/images/image.png)

Lastly, our inferential model determined the specific features that were most important in determining price, those being distance from Seattle and Redmond, living area in square feet, number of bedrooms, and room sizes.

## Conclusion
- To conclude, our predictive model can reasonably predict the sale price of a house with a typical error of 160 thousand dollars.

- Beyond the predictions of our model, Lake and Company should most closely pay attention to distance from city centers, livable area in square feet, number of bedrooms, and room sizes.

- Ultimately, we recommend more data collection and more advanced modeling in order to further improve and refine these results.

## For More Information
View our full [Jupyter Notebook](https://github.com/UpGoerFive/King-County-Project/blob/master/Combined-Notebook.ipynb) and/or see our [presentation slides](https://github.com/UpGoerFive/King-County-Project/raw/master/Selling%20houses%20in%20the%20seattle%20area.pdf).
