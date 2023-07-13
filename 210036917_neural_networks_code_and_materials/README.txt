Dependencies:
Python:
pandas
numpy
matplotlib.pyplot
seaborn
statsmodels
sklearn
optuna
plotly
torch
skorch

EDA is done in the diabetes5050_EDA.ipynb file, which imports the diabetes_binary_5050split_health_indicators_BRFSS2015.csv dataset, 
completes EDA and preprocessing, before saving the processed dataset as processed_diabetes5050_dataset.csv.

The hyperparameter tuning is done in the diabetes5050_neural_nets.ipynb file. The file does a train test split and the training and
test sets are saved in the final_models file. Once hyperparameters have been tuned, the models are trained with those hyperparameters,
and the trained models are saved in the final_models folder as pickle files.

Testing the final models happens in the final_model_tests.ipynb file. The trained final models are imported from the final_models folder
before being tested on the test sets, which are also imported from final_models. Confusion matrices, precision, recall, F1 scores and ROC
curves are plot for the final model.

Graphs obtained from EDA are in the EDA_graphs folder.
Graphs obtained from hyperparameter tuning are in the hyperparameter_tuning_graphs folder.
Graphs obtained from the final models are in the final_graphs folder.
