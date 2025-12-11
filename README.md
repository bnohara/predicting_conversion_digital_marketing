<h1>Summary and Goal</h1>
<p>In this project, we look at marketing campaign data at the user level. The goal is to create a machine learning model to predict which users will <b>not</b> convert.</p>

<p>Conversion rate in this dataset is pretty high at 88%, so identifying the minority case should be more useful. To increase campaign efficiency, these non-converting users could be added to an exclusion audience. Or, experiments could be run with different marketing strategies to see how to increase the conversion rate for these users.</p>

<h1>Results</h1>
<p>An ensemble stacking classifier of the following performed the best: LightGBM, XGBoost, CatBoost, Gradient Boosting, and AdaBoost.</p>

<p><b>Our initial goal was to predict non-converters, and we did this with an F1 score of 0.72.</b> This is likely the more valuable use case.</p>

<p>Still, <b>F1 score for predicting converting users was also high at 0.97</b>, so the model does increase our intelligence at predicting the majority case as well.</p>

<h1>Next Steps</h1>
<p>To further improve the model, particularly for the non-converting user case, these strategies could be tested:
<ul>
<li>Adding aggregation features like gender x age group, total page visits, time spent per page, etc
<li>Removing low importance features, identified by mutual information
<li>More robust hyperparameter tuning with Optuna
</ul>
</p>

<h1>Data Source</h1>
Kaggle: https://www.kaggle.com/datasets/rabieelkharoua/predict-conversion-in-digital-marketing-dataset/data
