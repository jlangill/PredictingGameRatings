# PredictingGameRatings
Using Kmeans to Predict Game Ratings

Read board_games.csv into a Dataframe called board_games using the pandas library.
Display the first few rows of board_games and get familiar with the data set.
Use the DataFrame.dropna() method to remove rows containing missing values.
Remove any rows that have no reviews.

Become familiar with the distribution of average ratings by generating plots and calculating summary statistics. For each of the following, write down your observations in a Markdown cell.
Generate a histogram of the average ratings.
Generate a box and whisker plot of the average ratings.
Calculate the standard deviation.
Calculating the mean.
Think about what error metric might make sense for this data, and write a markdown cell with your thoughts.

Use the DataFrame.corr() method to compute pairwise correlations between only the numeric columns. Assign the result to correlations.
Display the average_rating column of correlations, which shows how much the other columns correlate with the average_rating column.
Do any of the correlations surprise you? Write up your thoughts in a markdown cell.
Remove any columns that seem to be derived from the average_rating. The bayes_average_rating is an example of this.
Remove any columns that don't seem to correlate at all with the average_rating column.

Initialize a LinearRegression model, and assign it to the variable reg.
Use the LinearRegression.fit() method to set the predictor columns you want the model to use and set the target column to average_rating.
Use the LinearRegression.predict() method to make predictions using the columns of board_games that you think should be used as predictors.
The predictors you pass into LinearRegression.predict() should be the same predictors you passed into LinearRegression.fit.
Assign the result to predictions.
Calculate the error metric that you chose earlier.
Write up what the error value tells you in a markdown cell.
