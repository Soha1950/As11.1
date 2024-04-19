
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

![image](https://github.com/Soha1950/As11.1/assets/160794678/156636bc-0dd9-4308-b00c-e19f1cf652e3)

The histogram of vehicle age shows the distribution of ages of vehicles in the dataset. From the plot, we can observe the following:

Most of the vehicles in the dataset are relatively young, with ages ranging from 0 to around 20 years.
There are fewer vehicles with ages between 20 and 40 years.
Only a small number of vehicles have ages greater than 40 years.
This distribution provides insights into the age distribution of vehicles in the dataset, which can be valuable for understanding the 





