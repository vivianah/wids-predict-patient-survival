# Prediction Patient Survival in the Intensive Care Unit (ICU)

This is the repository for the WIDS 2020 Kaggle competition where we use patient information to predict their dealth probability in the first 24 hours at the ICU.


## Getting Started

This project requires Python 3.7 and the following Python libraries installed:

* NumPy 1.16.5
* Pandas 1.3.1
* matplotlib 3.1.1
* scikit-learn 0.22
* seaborn
* lightgbm
* imblearn


## Running the Code

All our finalized notebooks are in the "notebooks/Finalized" folder. Please run the jupyter notebook in the order of step numbers in title. 

1. Run __Step1_WIDS+EDA.ipynb__ - 
   This is our EDA process.

2. Run __Step2_WIDS_Feature_Engineer_0309.ipynb__ - 
   We created additional features.

3. Run __Step3_lightgbm_baselinemodels.ipynb__ - 
   We built a basedline model by only using the raw and unimputed dataset.

4. Run __Step4_Model_Iterations.ipynb__ - 
   We ran three models plus resampling methods on our imputed dataset.

5. Run __Step5_LGB_U_Hyperpara_Tuning.ipynb__ - 
   We tuned hyperparameters of our finalized model. NOTE: Please DO NOT RUN the notebook beginning at the "Submit to Kaggle" portion as that is only for the purposes of our own validation. Thanks!

6. Run __Step6_Probability Calibration.ipynb__ - 
   We tried calibrating our probability threshold.

## Data

The original data can be found in "data" folder. This includes the following files:

1. __trainingv2.csv__ : Our training data with 91,713 oberservations and 185 features. 
    The target variable "hospital_death" is a binary variable where 1 indicates death and 0 indicates survival.
    
2. __icu-apache-codes.csv__ : Map to match APACHE III diagnosis codes with their parent chronic condition.

3. __unlabeled.csv__ : The holdout unlabeled data used to predict survival
