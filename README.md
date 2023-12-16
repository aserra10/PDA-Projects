### Project 1: Exploring the Link between Smoke Exposure During and After Pregnancy On Adolescent Substance Use, Self-Regulation, and Externalizing Behaviors

The exploratory analysis on the effects of smoking during pregnancy (SDP) in adolescent substance use, self-regulation, and externalizing behaviors in this project is motivated by a study conducted by Markham Risica et al. This study focused on low-cost interventions aimed at decreasing Environmental Tobacco Exposure (ETS) during and after pregnancy. For this project, data used in this exploratory analysis comes from a current study being undertaken by Dr. Lauren Micalizzi, with a focus on outcomes in adolescents whose mothers who smoked during pregnancy. This study includes data on 100 mothers with children ages 12 to 16 years old. Data collected are baseline, 6-month, and 12-month laboratory sessions, computerized self-regulatory assessments, self-reported substance use, self-regulation, and other parent and child self-report of other relevant behaviors. In this project, only a sample of the data was used.

In a short overview of the results, adolescent outcomes tended to be worse in terms of externalizing and internalizing behaviors scores for those whose mothers engaged in smoking behaviors during their entire pregnancy. These adolescent also had a higher percentage who engaed in some type of substance use. For mothers who were exposed to ETS post-pregnancy, there was no clear pattern observed. Substance use and externalizing behaviors scores among adolescents were highest for those who mothers reported not being exposed to ETS, and internalizing behavior scores were highest for mothers reporting to have been exposed to ETS for 4 to 5 years post-pregnancy. 

![sdp_p1](https://github.com/aserra10/PHP2550-Projects/assets/119968598/f268fd7c-b77c-4ced-8573-54f48a270ea6)

![ETS_p1](https://github.com/aserra10/PHP2550-Projects/assets/119968598/fb63797f-349c-42f0-8d45-e5a0642aecff)


For this project see the following files: 
- The *pda_project.R* file provided by the instructor merged study data of both parent and child into a new dataset containing parent ID as a unique identifier.
- An exploratory data analysis was conducted in the *Project_1_as.rmd* file. See corresponding pdf file for easy viewing.
- For data privacy purposes, the dataset was not included in the repository.
  
## Project 2: Developing Prediction Models for Tracheostomy in Infants with Severe Bronchopulmonary Dysplasia
This project focuses on a dataset that includes baseline and demographic characteristics in addition to respiratory support information at 36 and 44 weeks PMA for infants born at or earlier than 32 weeks PMA who are at higher risk for BPD. Severity of BPD categories (Mild, Moderate, Severe) at week 36 PMA were coded using the NHLBI(2018) definition. The project two file includes code conducting a thorough examination of five tracheostomy outcome prediction models, employing four different fitting methods to select the most effective model. These four fitting methods are coded through functions: lasso, ridge, and logistic forward and logistic backward. Models undergo evaluation using positive and negative predictive value comparison, accuracy, AUC measure, and coefficient estimates. Packages needed for this evaluation are listed at the top of the file including pROC. Using the mice package in R, 5 imputed train and test datasets were generated. The models were fit on the training data and validated on the test data. The results showed that the lasso model with two-way interactions consistently outperforms its counterparts, demonstrating better predictive accuracy compared to all other fitting models. All statistical analyses were performed using R Version 4.3.1. 

# Project 3: Transportability Analysis of the Framingham ATP-III Prediction Model
This study assesses the transportability of the Framingham ATP-III model when transported from the source population on which it was developed to a new target population. Examining the performance of a model when being applied to a new target population, often with different characteristics than the source population, is important to gain a better understanding of how well the model performs
in a different setting. The transportability analysis for this model was conducted through a Monte Carlo simulation with 500 repetitions where Framingham study data was used as the source and simulated NHANES data as the new target population. Performance of this predictive model was assessed using the brier score as defined in Steingrimsson et al., using an inverse-odds weighting estimator. Our results showed the mean brier estimate for men was slightly higher than the estimate for women, but overall the bias of the simulation brier estimate was relatively low for both men and women in reference to the “true” estimated from the non-simulated data. 

The following plot shows an example of correlations from the simulated data for men. 
![sim_corr_p3](https://github.com/aserra10/PHP2550-Projects/assets/119968598/26ecffff-11f5-48d2-acb2-182e76f438e3)

The tables below show the brier score estimates for men and women from the simulation.
![p3_est2](https://github.com/aserra10/PHP2550-Projects/assets/119968598/b6f4a4ba-bfb1-409a-a677-6ef892531b40){:width="300px"}
![p3_est](https://github.com/aserra10/PHP2550-Projects/assets/119968598/1743cb33-66d3-45f7-8f8b-d035a081661f){:width="300px"}

For this project see the following files: 
- The *Project_3_as.RMD* file includes code for the simulation and estimation of brier scores. It also includes the required packages and references. See the corresponding pdf file for easier viewing.
- The data used in this project is publicly available and can be accessed through R. See code for more details.


