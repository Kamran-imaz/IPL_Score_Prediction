# IPL_Score_Prediction

## Introduction
This Project is a Machine Learning Project which aims to Predict the score of the team based on certain parameters. The project uses a dataset containing ball-to-ball information from Season-1 to Season-10. download the dataset [here](https://www.kaggle.com/datasets/yuvrajdagur/ipl-dataset-season-2008-to-2017). This Project adapts various <span style="color:red; font-weight:bold;">**Regression Algorithms**</span> to predict the score.

## Data-Preprocessing
The data is preprocessed by removing unnecessary columns (manually), followed by removing the teams which do not play frequently and then converting them into numerical variables with the help of <span style="color:red; font-weight:bold;">**string indexing**</span> followed by <span style="color:red; font-weight:bold;">**one-hot encoding**</span>. and then followed by applying <span style="color:red; font-weight:bold;">**principal component analysis**</span> to check if there are any unwanted columns (low variance).

## Model Results
<img width="448" alt="3" src="https://github.com/user-attachments/assets/5bfc38ad-9b4d-4b1a-97aa-ab5d6f234035">

## Data Training and Testing
This involved implementing four regression models (Linear, Decision tree, Random forest and Gbt Regressor). Cross-validator is used along with hypertuning of the parameters to avoid overfitting. and then they were stacked together once with GBT and with Linear Regression.

## Model Evaluation
All the models were evaluated with the help of RMSE(Root Mean Square Error). Out of them GBT Regressor Performed very well before stacking and after stacking as well.

## References
- [Dataset](https://www.kaggle.com/datasets/yuvrajdagur/ipl-dataset-season-2008-to-2017)
- [Pyspark](https://spark.apache.org/docs/latest/api/python/index.html)
- [Hyperparameter Tuning](https://www.geeksforgeeks.org/hyperparameter-tuning/)
