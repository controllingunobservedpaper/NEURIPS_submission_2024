# neurips_submission_2024

### This is the submission for NeurIPS 2024.

This repository includes neurIPS_submission_file.ipynb, tte_categorical_mcsimex.ipynb, and requirements.txt.

The neurIPS_submission_file.ipynb notebook contains the derivations, calculations, and experimentations to account for measurement error w.r.t an originally "unknown" and imputed (via LLMs such as BERT) confounder (ex: Smoking Status) in causal effects (specifically risk and odds ratio). It is important to note that due to privacy rules with MIMIC-III and Harvard's n2c2 2006 smoking dataset, it is not possible to show certain components of the processs (ex: data filtering, dataframe generations, model training, etc...). However, some information about the dataframes are given within comments in the notebook, such as number of rows/columnss and important feature names to help viewers better understand the flow for causal analysis, especially with creating formula strings. Additionally, pickle files (such as the files containing separate varied error matrices) used for bootstrapping are not included in this notebook, but the process of using them to measure the variance of causal effects is still demonstrated.

The tte_categorical_mcsimex.ipynb contains the calculations for risk ratio when utilizing MC-SIMEX. This notebook is in R.