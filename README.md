# Know Your Ship
From data to containership performance. Unleash the potential of machine learning.

The next big challenge our society is facing today is to reduce CO2 emissions. Therefore, the shipping industry strives to reach the net-zero target by 2050. 
In order to contribute to this goal, the team analysed a container ship dataset from Hapag-Lloyd and built a model to predict the fuel consumption of the main engine. The model highlights interconnections between variables and can be used for operational optimisation and forecasting. 

To accomplish this task, the data was provided via SQL databases and additional data was included. The enriched data was analysed and used to train a regression model with the acquired machine learning techniques from the bootcamp to predict the fuel consumption. Undergoing all stages of the data science life cycle, the project was finally presented to the stakeholder group.

Techstack:

SQL, Python, Numpy, Pandas, Machine-learning, MLFlow, Statsmodel, Sklearn, Seaborn, Plotly, Dashboard, API, Git



Table of Content:
* [Preprocessing](notebooks/01_Preprocessing_HFData.ipynb):
    Data was obtained in s3db format and had to be preprocessed in able to use it with pandas.
* [Engine model](notebooks/02_1_Engine_model.ipynb):
    Creation of the power prediction model based on CFD calculations.
* [Featureengineering](notebooks/02_2_Featureengineering.ipynb):
    Additional Features were created. Combination with daily noon report and engine model.
* [EDA tools](notebooks/03_EDA_Tools.ipynb):
    Tools used for the EDA.
* Models: Different models were used and evaluated with MLFlow:
    * [Random Forest](notebooks/04_1_Model_Random_Forrest.ipynb)
    * [Stacking](notebooks/04_2_Model_Stacking.ipynb)
    * [Regression Tree](notebooks/04_3_Model_Regression_Tree.ipynb)
    * [KNN](notebooks/04_4_Model_KNN.ipynb)
    * [Linear Regression with Polynomial Features](notebooks/04_5_Model_Linear_Regression_Polynomial.ipynb)
    * [OLS](notebooks/04_6_Model_OLS.ipynb)
    * [Gradient Descent](notebooks/04_7_Model_Gradient_descent.ipynb)
    * [SVM](notebooks/04_8_Model_SVM.ipynb)
* [Clustering](notebooks/05_Clustering.ipynb):
    Passages were clustered to gain more insights into differences.
    

## Requirements:

- pyenv with Python: 3.9.4

### Setup

Use the requirements file in this repo to create a new environment.

```BASH
make setup

#or

pyenv local 3.9.4
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements_dev.txt
```

The `requirements.txt` file contains the libraries needed for deployment.. of model or dashboard .. thus no jupyter or other libs used during development.
