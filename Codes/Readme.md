# RANDOM MODELS FOR THE JOINT TREATMENT OF RISK AND TIME PREFERENCES

by Jose Apesteguia, Miguel A. Ballester and Angelo Gutierrez-Daza

March 2020

This folder contains the data and Matlab codes necessary to replicate the
empirical exercises reported in section 6 of the paper.

The folder has three subdirectories, one for each dataset explored in the main
text of the paper:

1) **AHLR**: Contains the code and data of the exercises described in section
5.1 of the paper, which use data from Andersen et al. (2008). The code gives as
output Table 1 and Figures 1-3 in the paper.
2) **CL**: Contains the code and data of the exercises described in section 5.2
of the paper, which use data from Coble and Lusk (2010). The code gives as
output Table 2 and Figures 4-6 in the paper.
3) **AS**: Contains the code and data of the exercises described in section 5.3
of the paper, which use data from Andreoni and Sprenger (2012). The code gives
as output Table 3 and Figures 7-9 in the paper.

To replicate the tables and figures in the paper, execute the "RUN_" matlab
script in the corresponding subfolder.

The folder for each dataset has a similar structure, with a main "RUN_" script
and 4 subfolders:

- **RUN_X.m**: This is the main file and the only one that needs to be run to
replicate the results for the corresponding dataset in the paper. This file
calls the scripts that compute the estimates and associated standard errors of
each model, plots the PDFs and CDFs shown in the paper and exports the tables
with the results as a CSV and LaTeX table.

- **Input**: Has a MAT file with the corresponding dataset used in the
estimation exercises.

- **MainFunctions**: Contains several scripts that run the estimation and
computation of standard errors for a particular model. Each script returns the
estimates corresponding to one or several columns in the corresponding table of
this dataset. The folder also has scripts that create the different figures and
tables shown in the paper. The figures are exported as .eps files while the
tables are exported as a CSV and a TEX file.

- **AuxiliaryFunctions**: Contains several functions that are used by the main
scripts to carry out the estimation of the models. These include, among others,
the log-likelihood functions of the different models, the functions defining the
PDF, CDF and moments of the distribution of each behavioral trait, a function to
compute clustered robust standard errors, and a function by Victor Martinez
Cagigal used to export the results as a LaTeX table.

- **Output**: All figures and tables returned by the scripts will be stored in
this folder.

Each script and function has additional documentation and further reference can
be obtained by consulting them directly.

All codes have been tested in Matlab 2019b using a laptop with 16GB of RAM and a
Intel Core i7 2.11 GHz processor. Reproducing all tables and figures in the
paper corresponding to the AHLR and CL datasets takes less than 3 minutes each.
Reproducing all tables and figures corresponding to the AS dataset takes 45
minutes.

## References

- Andersen, Harrison, Lau and Rutsrom (2008),*"Eliciting Risk And Time
Preferences"*. Econometrica.

- Coble and Lusk (2010).*"At the nexus of risk and time preferences: An
experimental investigation"*. Journal of Risk and Uncertainty.

- Andreoni and Sprenger (2012). *"Estimating Time Preferences from Convex
Budgets"*. American Economic Review.
