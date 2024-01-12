Business Data Challenge
Companies in the entertainment industry nowadays face a substantial risk: Large upfront investments are often necessary for movie productions, but only 20% of movies end up being profitable (Forbes, 2019). Indicators are needed that help companies estimate the financial of their movie, make more informed decisions and so are able to mitigate the risk of loosing money on a movie project. To enhance the movie production company's chances of producing profitable films the use of data analytics is crucial . By analyzing historical data on movie sucess, trends, correlations, and patterns can be uncovered and used to make informed decisions regarding genre, casting, or marketing strategies. Utilizing machine learning algorithms, our predictive models will be able to forecast potential box office performance and allow to optimize resources and achieve maximum profitability.Predicting income can be insightful when evaluating a movie's financial success because it gives an estimate of the total revenue generated by the movie. While profit and ROI are important metrics for measuring financial success, they are dependent on multiple factors beyond just the revenue generated by the movie. For example, profit depends on the movie's budget, marketing costs, distribution fees, and other expenses.
On the other hand, predicting income provides a straightforward estimate of the revenue generated by the movie, which can be compared to the movie's budget to determine whether it was financially successful. Additionally, predicting income can help in forecasting the potential revenue that a movie might generate in the future.
Overall, predicting income from a movie database can be a useful tool in evaluating a movie's financial success as it provides a clear picture of the movie's revenue generating potential.

Feature Engineering
Before the models will be trained 'Dummy Variables' are created for 'Categorical Variables'. Furthermore, highly correlated features are excluded (e.g. certain filming locations) and the numerical variables with skewed distributions, including the target variable were log transformed. The dataset is split into 80% training and 20% test data to later evaluate the performance of the model.OLS Regression
Investigating variables with significant p-values serves to analyze their importance for predicting income. Their coefficients indicate whether those variables have negative or positive impact on the target variable. Due to the log transformation the scale of the variables may not be absolute, but the coefficients can still be used to understand the direction and magnitude of their impact on the target variable.The model selection is based on the business objective, which is to provide insights into the factors that drive a movies financial performance. Interpretable models can provide clear insights into these factors. Moreover, performance metrics, such as mean absolute error, MAPE, and R squared server to evaluate the model.Analyzing Coefficients, features importances as indicated by the Random Forest and looking at the decision Tree, the following features are important for a movies' financial performance: Runtime, Budget, Certificate, Certificate_TV-PG, Stars_class, Filming_location_Serbi, Country_of_origin_USA, and different Genre, including Drama, Western, Animation, and Adventure. These insights also inspired going into some more depth in the Data Analysis insights that are mentioned above.

Practical Implications
As moderate budget movies do not seem to achieve much higher profits than low budget productions, it is not worth to have a medium budget movie, either try to keep the budget low or go big.
The profitability of a movie seems to be increasing with higher profile actors in them, so logically casting more famous actors promises more financial success.
Make movies longer and try to not receive an age restriction
The best performing model explains about 50% of the variance in the dependent variable, which means that there is still a huge potential to uncover more factors that contribute towards the financial performance of a movie.

Limitations
As the best r2 score suggests, there are many other factors influencing the financial performance of these movies. Therefore, the insights should be taken as absolutes. Moreover, the analyisis is based on correlation not causation, a fact often being overshadowed.
The decision Tree is not transformed back to the original scale. So as of now it is only useful for extracting the features that are split on, but not what the cut-offs are for Budget and Runtime.
I might be interesting to further explore the movie titles, which have been left out for this analysis
