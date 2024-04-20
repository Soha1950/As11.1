
1. Business Understanding Phase:
Identify the requirements and constraints of the used car dealership.
The goal is to build a predictive model that can estimate the price of a used car based on its characteristics, such as 'year', 'manufacturer', 'model', 'condition', 'cylinders', 'fuel', 'odometer', 'transmission', 'drive', 'size', 'type', 'paint_color', and 'state'.


2. Data Understanding Phase:
During the data understanding phase, I examined a dataset that contains information on used cars. This includes assessing data quality through various visualizations, examining correlations and relationships between features, and identifying anomalies or issues in the dataset.

3. Data Preparation Phase:
During the data preparation phase, I refined the dataset by cleaning it, standardizing, and constraining the price column between 200,000 and 400,000 to form the final dataset appropriate for analysis. Additionally, I performed tasks such as managing missing values, encoding categorical variables, scaling numerical features, and rectifying data by addressing missing values, outliers, and inconsistencies

4. Modeling Phase:
 Linear Regression, Decision Tree Regression, and Random Forest Regression. Here are the Mean Squared Error (MSE) values obtained for each model:

Linear Regression:

Mean Squared Error: 0.06756854315775475
Decision Tree Regression:

Mean Squared Error: 0.006712767229488695
Random Forest Regression:

Mean Squared Error: 0.012299407487930819
Lower values of MSE indicate better model performance, as they represent a smaller difference between the predicted and actual prices. Based on the MSE values, it appears that the Decision Tree Regression model performs the best among the three models, as it has the lowest MSE

5. Evaluation Phase:
 In the evaluation stage, I assessed the efficacy of the trained regression models utilizing the mean squared error (MSE) evaluation metric. Consequently, the decision tree model demonstrated good performance in predicting the car prices.

6. Deployment Phase:
Utilizing the decision tree model to inform the pricing strategy for the second-hand car agency, I discerned crucial insights. Within this model, the odometer feature and the car model emerged as pivotal factors influencing pricing decisions. However, upon transitioning to the random forest regression model, the significance shifted towards the odometer and car color features. Conversely, the linear regression model produced markedly distinct outcomes, including instances of negative values. Notably, the year of manufacture and the condition of the vehicle surfaced as primary considerations within this model's framework. This nuanced understanding underscores the multifaceted nature of the pricing dynamics and highlights the necessity of employing diverse analytical approaches to extract comprehensive insights for informed decision-making






![image](https://github.com/Soha1950/As11.1/assets/160794678/85b44635-1c10-467e-acc3-6175a8e0956f)

Pairplot of Numerical Variables:

The pair plot provides a visual representation of the relationships between pairs of numerical variables, including 'id', 'price', 'year', and 'odometer'. From the pair plot, we can observe:
There doesn't seem to be a clear linear relationship between 'id' and other numerical variables.
There appears to be a positive correlation between 'price' and 'year', indicating that newer vehicles tend to have higher prices.
There is a negative correlation between 'price' and 'odometer', suggesting that vehicles with lower mileage tend to have higher prices.
'year' and 'odometer' don't seem to have a strong linear relationship based on the scatter plots.

![image](https://github.com/Soha1950/As11.1/assets/160794678/50769aeb-66a2-4c11-96ff-bd857327de70)

Histogram of price:

The histogram of 'price' shows the distribution of vehicle prices in the dataset. It appears that the majority of vehicles have prices clustered around the lower end of the price range, with a few outliers at higher prices. This distribution might suggest that most vehicles in the dataset are relatively affordable, with a few luxury or high-value vehicles.


![image](https://github.com/Soha1950/As11.1/assets/160794678/6fc9ceab-0be4-4c0e-8d52-540a6f536ee0)

Histogram of year:

The histogram of 'year' indicates the distribution of vehicle model years. It shows that there are more recent vehicles in the dataset, with a peak around the years 2015-2020. This distribution suggests that the dataset contains a significant number of newer vehicles compared to older ones


![image](https://github.com/Soha1950/As11.1/assets/160794678/b1e7951b-e80d-4c03-b32a-c496c8762d4b)

Histogram of odometer:

The 'odometer' histogram displays the distribution of vehicle mileage. It indicates that many vehicles in the dataset have low mileage, with a peak at the lower end of the odometer range. This distribution suggests that the dataset contains a mix of both low-mileage and high-mileage vehicles, with more vehicles having lower mileage.





The plot shows individual data points for each car, where each point represents a combination of odometer reading and price.
The distribution of data points suggests the spread of prices across different odometer readings, indicating the variability in car prices based on mileage.
Trend:

From the plot, we can observe whether there is any discernible pattern or trend between odometer reading and price. For example, we might expect older cars with higher mileage to be priced lower compared to newer cars with lower mileage.


The histogram of vehicle age shows the distribution of ages of vehicles in the dataset. From the plot, we can observe the following:

Most of the vehicles in the dataset are relatively young, with ages ranging from 0 to around 20 years.
There are fewer vehicles with ages between 20 and 40 years.
Only a small number of vehicles have ages greater than 40 years.
This distribution provides insights into the age distribution of vehicles in the dataset, which can be valuable for understanding the composition of the vehicle population and for further analysis or modeling tasks.


![image](https://github.com/Soha1950/As11.1/assets/160794678/41e34c3d-5ded-4320-ab44-6d6913047a24)

In this bar chart illustrating feature importances derived from the Linear Regression model, the title status feature once again emerges as the most influential determinant of used car prices. Following closely are the condition, type, and fuel type of the vehicle, which continue to demonstrate substantial importance in price estimation.

Interestingly, similar to the Random Forest Regression model, the odometer reading displays a negative importance in the Linear Regression model as well. This suggests that while mileage traditionally plays a crucial role in determining car prices, its significance may be diminished or even reversed under certain circumstances, as indicated by this model.

Other features such as VIN, paint color, and model maintain moderate importance, while regional and manufacturer factors exhibit relatively lower importance, consistent with the findings from the Random Forest Regression analysis. This nuanced understanding of feature importance underscores the multifaceted nature of pricing dynamics in the used car market, enabling stakeholders to make informed decisions when devising pricing strategies and assessing the value of vehicles.


![image](https://github.com/Soha1950/As11.1/assets/160794678/d00e45df-a52c-4a04-a55d-64a631626dbf)

In the bar chart representing feature importances obtained from the Decision Tree Regressor model, the paint color feature emerges as the most influential factor affecting used car prices. This highlights the significance of aesthetics and personal preferences in shaping consumer decisions within the automotive market.

Following closely behind are the VIN (Vehicle Identification Number) and odometer reading, both of which hold substantial importance in pricing determination. These features provide crucial insights into the vehicle's history and usage, thereby influencing its perceived value in the market.

Manufacturer, region, and vehicle type also exhibit notable importance, suggesting that factors such as brand reputation, geographic location, and vehicle category play significant roles in price variability. Additionally, the model of the car holds moderate importance, underscoring the impact of specific vehicle models on pricing dynamics.


![image](https://github.com/Soha1950/As11.1/assets/160794678/6ec49e29-d8d7-4f4d-8800-58e630bc41dc)


In the feature importances chart generated from the Random Forest Regression model, the VIN (Vehicle Identification Number) feature stands out as the most significant determinant of used car prices. This underscores the importance of vehicle history and individual identification in influencing pricing decisions within the automotive market.

Following VIN, the odometer reading emerges as the second most influential factor. This aligns with common expectations, as mileage often serves as a key indicator of a vehicle's wear and tear, directly impacting its perceived value in the secondary market.

The year of manufacture also holds considerable importance, reflecting the market's tendency to assign higher values to newer vehicles. This highlights the role of vehicle age in pricing dynamics and consumer preferences.

Other features such as car model, region, and paint color exhibit moderate importance, suggesting their influence on pricing variations. Additionally, factors like transmission type, state, and vehicle condition contribute to the overall understanding of pricing determinants, albeit to a lesser extent.

Overall, this analysis provides valuable insights into the factors driving used car prices, enabling stakeholders to make informed decisions in pricing strategies and market positioning.


Other features such as transmission type, year of manufacture, and vehicle size maintain relatively lower importance but still contribute to the overall understanding of pricing determinants in the used car market. This comprehensive analysis of feature importances facilitates a deeper understanding of the key drivers behind pricing variations, empowering stakeholders to make informed decisions in pricing strategies and market positioning.


![image](https://github.com/Soha1950/As11.1/assets/160794678/c3417dcf-8a64-4c16-a6e8-4638b7029044)

I have applied three different regression models to my data and evaluated their performance using cross-validation. Here is a summary of the results:

Linear regression:
Crossover R-squared score (CV R2): 0.484
Mean square error: 0.038
Decision Tree Regression:
CV score R2: 0.004
Mean squared error: 0.07
Random Forest Regression:
CV score R2: 0.055
Mean squared error: 0.06
Let's interpret these results:

Linear regression:
The CV R2 score of 0.484 indicates that the linear regression model explains approximately 48.4% of the variance of the target variable. This indicates a moderate level of predictive power.
The mean squared error is relatively low at 0.038, indicating that the model predictions are generally close to the true values.
Decision Tree Regression:
A CV R2 score of 0.004 indicates that the decision tree model explains very little of the variance of the target variable. It performs poorly in capturing basic patterns in the data.
The mean squared error is greater than 0.07 compared to linear regression, which indicates a greater difference between the predicted and actual values.
Random Forest Regression:
The CV R2 score of 0.055 indicates slightly better performance than the decision tree but is still relatively low compared to linear regression.
The mean squared error of 0.06 is similar to the decision tree, indicating that the predictions of the random forest model also have a significant margin of error.
Based on these results, it seems that the linear regression model is the most effective model among these three models in terms of prediction accuracy. If the decision tree model is not cross-validated, it is the best model.






