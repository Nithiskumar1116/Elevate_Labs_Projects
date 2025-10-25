# Movie_Success_Prediction_and_Sentiment_Study
Project 2 || Data Analyst Intern || Elevate Labs

The main goal of this project is to analyze the IMDB Top 1000 movies dataset to:
Understand patterns in movie ratings, audience engagement, and sentiments.
Identify how movie features such as rating, votes, and text sentiment relate to box office revenue.
Build a predictive model to estimate movie gross revenue.

Data Collection

Dataset used: IMDB_Top_1000.csv
Contains details such as:
Series_Title, Genre, IMDB_Rating, No_of_Votes, Gross, Meta_score, Overview, and more.

Data Cleaning and Preparation

Removed missing and duplicate values.
Cleaned the Gross column by removing $ and , symbols and converting it to a numeric format (Gross_num).
Extracted main genre from multi-genre fields (e.g., “Action, Adventure, Sci-Fi” → “Action”).
Handled null values in text and numeric columns.
Verified data consistency using descriptive statistics and null value checks.

Sentiment Analysis

Applied VADER Sentiment Analyzer to the Overview column to evaluate each movie’s textual sentiment.

Generated two new columns:
overview_compound: Sentiment score (range: -1 to +1).
overview_sentiment: Sentiment category (positive, neutral, negative).

Interpreted results to understand audience perception based on overview tone.

Data Visualization

Created several insightful visualizations using Matplotlib and Seaborn:
Sentiment Distribution: Count of positive, neutral, and negative overviews.
Genre-wise Sentiment: Average sentiment score by genre.
Rating vs Sentiment: Explored how higher-rated movies correlate with more positive overviews.
Gross vs Sentiment: Observed that movies with positive sentiments tend to earn higher gross.

All visualizations were saved as PNG images and embedded into the Excel report.

Predictive Modeling

Built a Linear Regression model to predict Gross_num using:
IMDB_Rating
No_of_Votes
overview_compound
Data was split into 80% training and 20% testing sets.

Evaluated model using:

R² Score: Measures variance explained by the model.

MAE (Mean Absolute Error): Average prediction error.

Example result:
R² Score = 0.62
MAE ≈ 15 million

This means the model explains about 62% of the variance in movie gross revenue.

Results and Insights

Movies with higher ratings and more votes tend to generate higher box office revenue.
Positive sentiments in movie overviews have a mild but positive correlation with revenue.
Genre trends: Adventure and Drama genres show higher sentiment averages and box office performance.
The model works reasonably well as a baseline and can be improved using transformations or advanced algorithms (like Random Forest or XGBoost).

Export and Reporting

Cleaned dataset, model summary, and all visualizations were exported to an Excel file:
IMDB_Cleaned_Analysis.xlsx

Separate sheets include:
>Cleaned_Data
>Model_Summary
>Graphs

Visuals and metrics embedded for easy reference and presentation.

Conclusion

This project successfully demonstrates how data preprocessing, sentiment analysis, and predictive modeling can be combined to analyze movie performance.
The analysis provides valuable insights into how audience ratings, engagement, and overview sentiments influence box office outcomes.
