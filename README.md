## Climate Change with ClimateWins

#### Project Overview

ClimateWins, a fictitious non-profit organization, seeks to apply machine learning (ML) to predict the consequences of climate change in Europe and beyond. It is concerned with the acceleration of extreme weather events in recent decades, believing that such fat-tailed risk can be viably modeled and predicted with ML.

#### Scope

Timeframe: *Jan 1960 - Oct 2022*

European Weather Stations: *Basel, Oslo, Stockholm, Budapest, Debilt, Dusseldorf, MunchenB, Madrid, Belgrade, Ljubljana, Heathrow, Maastricht, Sonnblick.*

Omitted (from project interim analysis): Valentia, Kassel, Roma, Gdansk, Tours.

#### Project Goal

For the interim report: fit three unsupervised ML models (K-Nearest Neighbors *aka* KNN, Decision Tree and Artificial Neural Network *aka* ANN) to temperature-based features time series data, as a classification prediction exercise on daily binary Pleasant/Unpleasant weather outcomes at the weather stations.

#### Data Sources

Weather data: European Climate Assessment & Dataset project

Pleasant Weather answers dataset: Origin not disclosed to the author.  (Red flag.)

#### Tools

•	Languages & Libraries: Python (Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, Plotly, Operator, Os, Tensorflow, Graphviz, Statsmodels, Datetime, Pylab, Mpl_toolkits)

•	Software: Jupyter Notebooks, Excel

#### Techniques Used

•	Data wrangled, merged, grouped, aggregated, summarized, transformed (first difference percentages, z-score normalization)

•	Time series data preprocessed, decomposed, stationarity-tested (ADF & KPSS tests, ACF plots), stationarized

•	Supervised learning: KNN, Decision Tree & ANN models deployed for classification prediction exercise

•	Hyperparameter optimization via GridSearchCV, model fine-tuning & regularization to minimize overfit on training data

•	Data visualized in Python (3D & 2D plots)

#### Attribution

OpenAI's ChatGPT, powered by GPT-4o, was enlisted for ML model customization, fine-tuning and regularization Python code and de-bugging; and for constructive criticism on model output.

#### Key Findings


•	The ANN bested the Decision Tree and KNN models on the *dodgy* Pleasant/Unpleasant Weather answers dataset classification prediction exercise, achieving a mid-60s Balanced Accuracy % score (on a 75/25 imbalanced class), minor slippage between Train & Test on Recall and Precision scores for each class, and ~1.3% Train-Test learning curve gap for Balanced Accuracy % score, suggesting low overfit.

•	Overall, there was likely an invisible performance "ceiling" faced by all models, due to the fact that the classification exercise placed a major constraint on feature inputs: only temperature-based features (min, max, mean) were permitted.  Even though present in the weather dataset, other features such as precipitation, cloud cover, wind velocity, humidity, etc. were disallowed as prospective data inputs.


•	If the feature-constraint were removed, the author believes the ANN and Decision Tree models can easily outperform current results.


#### Folders

•	01 Datasets: Original, processed and split data files.  Original weather data is in the "Dataset-weather-prediction-dataset-processed.xlsx" Excel file.  Pleasant/Unpleasant Weather answers data is in the "Dataset-Answers-Weather_Prediction_Pleasant_Weather.xlsx" Excel file of unknown provenance.

•	02 Scripts: Python scripts for the sequential stages of the project, differentiated by topics.  The Task 1.5 folder file named "ML Task 1.5 part 2 - Summary Results - DT vs ANN models" has tables highlighting model-vs-model results.

•	03 Project Management: Project Brief, pdf format.

•	04 Interim Report: Project interim summary, pdf format.
