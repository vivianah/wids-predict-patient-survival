<<<<<<< HEAD
# Prediction Patient Survival in the Intensive Care Unit (ICU)

This is the repository for the final project for the MSCA Data Mining Course where we use patient information to predict their dealth probability in the first 24 hours at the ICU.


## Getting Started

This project requires Python 3.7 and the following Python libraries installed:

*NumPy 1.16.5
*Pandas 1.3.1
*matplotlib 3.1.1
*scikit-learn 0.22
*seaborn
*lightgbm
*imblearn


## Running the Code

All our finalized notebooks are in the "Finalized" folder. Please run the jupyter notebook in the order of step numbers in title. 

1. Run Step1_WIDS+EDA.ipynb
   This is our EDA process.

2. Run Step2_WIDS_Feature_Engineer_0309.ipynb
   We created additional features.

3. Run Step3_lightgbm_baselinemodels.ipynb
   We built a basedline model by only using the raw and unimputed dataset.

4. Step4_Model_Iterations.ipynb
   We ran three models plus resampling methods on our imputed dataset.

5. Step5_LGB_U_Hyperpara_Tuning.ipynb
   We tuned hyperparameters of our finalized model.

6. Step6_Probability Calibration.ipynb
   We tried calibrating our probability threshold.

## Data

The original data can be found in "Data" folder. This includes the following files:

1. __trainingv2.csv__ : Our training data with 91,713 oberservations and 185 features. 
    The target variable "hospital_death" is a binary variable where 1 indicates death and 0 indicates survival.
    
2. __icu-apache-codes.csv__ : Map to match APACHE III diagnosis codes with their parent chronic condition.

3. __unlabeled.csv__ : The holdout unlabelled data used to predict survival






=======
# Data Mining Project 2019

# Instruction
All our finalized notebooks are in the "Finalized" folder. Please run the jupyter notebook in the order of step numbers in title. Please note that since we reorgnized the repository, files' relative paths have change. If you encounter any error, please change the file path accordingly. 

1. Run Step1_WIDS+EDA.ipynb

This is our EDA process.

2. Run Step2_WIDS_Feature_Engineer_0309.ipynb

We created additional features. 

3. Run Step3_lightgbm_baselinemodels.ipynb

We built a basedline model by only using the raw and unimputed dataset.

4. Step4_Model_Iterations.ipynb

We ran three models plus resampling methods on our imputed dataset. 

5. Step5_LGB_U_Hyperpara_Tuning.ipynb

We tuned hyperparameters of our finalized model.

6. Step6_Probability Calibration.ipynb

We tried calibrating our probability threshold. 
>>>>>>> 1e7e3489edb6823e2ba8aa95883aacef7769ddd8
