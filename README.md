### Project 1: Exploring the Link between Smoke Exposure During and After Pregnancy On Adolescent Substance Use, Self-Regulation, and Externalizing Behaviors

The exploratory analysis on the effects of smoking during pregnancy (SDP) in adolescent substance use, self-regulation, and externalizing behaviors in this project is motivated by a study conducted by Markham Risica et al. This study focused on low-cost interventions aimed at decreasing Environmental Tobacco Exposure (ETS) during and after pregnancy. For this project, data used in this exploratory analysis comes from a current study being undertaken by Dr. Lauren Micalizzi, with a focus on outcomes in adolescents whose mothers who smoked during pregnancy. This study includes data on 100 mothers with children ages 12 to 16 years old. Data collected are baseline, 6-month, and 12-month laboratory sessions, computerized self-regulatory assessments, self-reported substance use, self-regulation, and other parent and child self-report of other relevant behaviors. In this project, only a sample of the data was used.

In a short overview of the results, the tables below show the average proportion of substance use, average usage within the past 30 days, and composite scores ranging from 0 to 1, with 1 being the highest indicated poor behavior. Adolescent outcomes tended to be worse in terms of externalizing and internalizing behaviors scores for those whose mothers engaged in smoking behaviors during their entire pregnancy. These adolescent also had a higher percentage who engaged in some type of substance use. For mothers who were exposed to ETS post-pregnancy, there was no clear pattern observed. Substance use and externalizing behaviors scores among adolescents were highest for those who mothers reported not being exposed to ETS, and internalizing behavior scores were highest for mothers reporting to have been exposed to ETS for 4 to 5 years post-pregnancy. 

![sdp_p1](https://github.com/aserra10/PHP2550-Projects/assets/119968598/f268fd7c-b77c-4ced-8573-54f48a270ea6)

![ETS_p1](https://github.com/aserra10/PHP2550-Projects/assets/119968598/fb63797f-349c-42f0-8d45-e5a0642aecff)


For this project see the following files: 
- The *pda_project.R* file provided by the instructor merged study data of both parent and child into a new dataset containing parent ID as a unique identifier.
- An exploratory data analysis was conducted in the *Project_1_as.rmd* file. See corresponding pdf file for easy viewing.
- For data privacy purposes, the dataset was not included in the repository.
  
### Project 2: Developing Prediction Models for Tracheostomy in Infants with Severe Bronchopulmonary Dysplasia
Bronchopulmonary dysplasia (BPD) remains a critical concern in neonatal health. According to Higgins et al., BPD is characterized by abnormal development of lung tissue which primarily affects preterm infants, leading to significant challenges in respiratory function. It is imperative for physicians to monitor the health trajectories of preterm infants to ensure they are receiving adequate care. In cases where an infant develops BPD, it is important know whether their condition evolves to the point of needing a tracheostomy. Receiving a tracheostomy in a timely manner can prevent worsening conditions and potentially avoid infant death.For this project, our analysis pertains to respiratory support information at critical time points, particularly at 36 weeks postmenstrual age (PMA), using a dataset that includes baseline and demographic characteristics in addition to respiratory support information at 36 and 44 weeks. Three tracheostomy outcome prediction models are fitted to the data, employing two different variable selection methods, a five-fold cross validation and backward model selection procedures, to select the most effective model. The results showed that the lasso model with two-way interactions consistently outperforms its counterparts, demonstrating better predictive accuracy compared to all other fitting models. The non-zero coefficients from the lasso two-way model included mainly interactions between center and other covariates. This draws attention to the differences between the centers that potentially influence the results. In moving forward, it would be of interest to consider a mixed-effects or multilevel model to account for the differences between centers. Besides center, many of the covariates also included ventilation support levels, peak oxygen levels, maternal race, and severity. The only main interactions included in this model were weight at 36 weeks and ventilation support level. Overall, these are possible variables of interest that may be helpful in predicting the need for a tracheostomy in infants which should be further investigated. The limitations of this project are expanded upon further in the files provided.

![image](https://github.com/aserra10/PHP2550-Projects/assets/119968598/5b5a0de9-92bf-4c7a-a31f-7b3361a933c5)


For this project see the following files: 
- The *Project_2_as.RMD* file includes exploratory data analysis of te data, code for the models fitted, and the resulting models. It also includes the required packages and references. See the corresponding pdf file for easier viewing.
- For data privacy purposes, the dataset was not included in the repository.
  
### Project 3: Transportability Analysis of the Framingham ATP-III Prediction Model
This study assesses the transportability of the Framingham ATP-III model when transported from the source population on which it was developed to a new target population. Examining the performance of a model when being applied to a new target population, often with different characteristics than the source population, is important to gain a better understanding of how well the model performs
in a different setting. The transportability analysis for this model was conducted through a Monte Carlo simulation with 500 repetitions where Framingham study data was used as the source and simulated NHANES data as the new target population. Performance of this predictive model was assessed using the brier score as defined in Steingrimsson et al., using an inverse-odds weighting estimator. The results showed the mean brier estimate for men was slightly higher than the estimate for women, but overall the bias of the simulation brier estimate was relatively low for both men and women in reference to the “true” estimated from the non-simulated data. This project highlights the possible transportability of a model developed on a source population to a new target population through simulated data, when the
outcome of interest is not observed and only summary level data for the target population of interest are available.


The following plot shows an example of correlations from the simulated data for men. 
![sim_corr_p3](https://github.com/aserra10/PHP2550-Projects/assets/119968598/26ecffff-11f5-48d2-acb2-182e76f438e3)

The tables below show the brier score estimates for men and women from the simulation.
![est](https://github.com/aserra10/PHP2550-Projects/assets/119968598/3921a729-d579-439d-a2d7-b5dfdf24f660)

![img2](https://github.com/aserra10/PHP2550-Projects/assets/119968598/2b0b95b2-5817-4bf5-835b-f62df00cf256)


For this project see the following files: 
- The *Project_3_as.RMD* file includes code for the simulation and estimation of brier scores. It also includes the required packages and references. See the corresponding pdf file for easier viewing.
- The data used in this project is publicly available and can be accessed through R. See code for more details.


