# Movie_Recommendation_System
Data Analysis Key Findings
The surprise library was successfully installed using pip.
Loading the 'ml-100k' dataset from surprise required downgrading NumPy to version 1.26.4 due to compatibility issues with NumPy 2.0.2.
Running package installation commands (%pip install) in separate code cells before executing code that depends on them is crucial in notebook environments.
Data preparation for the surprise library involves building a full training set using data.build_full_trainset() and then building a test set from the resulting trainset using trainset.build_testset().
A Singular Value Decomposition (SVD) model was successfully trained on the prepared training data.
The trained model's performance was evaluated, yielding an RMSE of approximately 0.6770 and an MAE of approximately 0.5362 on the test set.
Generating recommendations requires identifying items the user has not yet rated, predicting ratings for these items using the trained model, and sorting the predictions to find the top recommendations.
Insights or Next Steps
The RMSE and MAE values indicate the model has a reasonable level of accuracy in predicting user ratings, providing a baseline for further optimization or comparison with other algorithms.
To make the recommendations more user-friendly, the item IDs ('1' to '1682') should be mapped back to their actual movie titles using the provided dataset's item information file.
Analyze the scatter plot of predicted vs. actual ratings to identify potential biases in the model's predictions (e.g., consistently over- or under-predicting).
Investigate recommended items with significantly different predicted ratings to understand the factors influencing these predictions.
Visualizations
Here are the visualizations of the model's performance and recommendations:

Model Evaluation Metrics
Model Evaluation Metrics

Top Recommendations for a User
Top Recommendations

Predicted vs. Actual Ratings
Predicted vs Actual Ratings
