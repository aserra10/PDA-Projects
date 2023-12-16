# Project 1: Developing Prediction Models for Tracheostomy in Infants with Severe Bronchopulmonary Dysplasia

This repository contains two main files. The *pda_project.R* file provided by the instructor merged study data of both parent 
and child into a new dataset containing parent ID as a unique identifier. The new data had included variables relating to
socioeconomic status, parent smoking status during and after pregnancy at different
time points, parent and baby cotinine levels, children substance use, and externalizing and self-regulation
variables. 
The main objective of this project was to examine effects of smoking during pregnancy and environmental
Tobacco exposure on adolescent self-regulation, substance use, and externalizing. An exploratory data analysis
was conducted in the *Project_1_as.rmd* file contained in this repository. The file is sectioned into reformatting data, missing
data analysis, baseline characteristics, correlations, and tables focused on outcomes of interest stratified by exposure. Packages 
required for this analysis are loaded at the top of the file. For data privacy purposes, the dataset was not included in the repository.


# Project 2
This project focuses on a dataset that includes baseline and demographic characteristics in addition to respiratory support information at 36 and 44 weeks PMA for infants born at or earlier than 32 weeks PMA who are at higher risk for BPD. Severity of BPD categories (Mild, Moderate, Severe) at week 36 PMA were coded using the NHLBI(2018) definition. The project two file includes code conducting a thorough examination of five tracheostomy outcome prediction models, employing four different fitting methods to select the most effective model. These four fitting methods are coded through functions: lasso, ridge, and logistic forward and logistic backward. Models undergo evaluation using positive and negative predictive value comparison, accuracy, AUC measure, and coefficient estimates. Packages needed for this evaluation are listed at the top of the file including pROC. Using the mice package in R, 5 imputed train and test datasets were generated. The models were fit on the training data and validated on the test data. The results showed that the lasso model with two-way interactions consistently outperforms its counterparts, demonstrating better predictive accuracy compared to all other fitting models. All statistical analyses were performed using R Version 4.3.1. 

# Project 3
In this project, the performance of a predictive model developed in a source population was evaluated when applied to a new target population. This transportability analysis was evaluated through a MC simulation using data generated separately for men and women to create a target population. A target population was simulated by first generating
the continuous variables using the mvrnorm function from the
mvtnorm package in R. The simulation involved 1,000 repetitions, and for each repetition the brier score using an inverse-odds weighting estimator was calculated. A list of required packages and references to formulas for calculating these estimates are included in the proj3copy.RMD


