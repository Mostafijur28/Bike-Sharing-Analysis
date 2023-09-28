# Bike Sharing System
Developing a regression model for shared bike demand allows management to analyze variations in demand based on different features. This model-driven approach enables strategic adjustments to meet customer expectations and optimize business strategies. Additionally, the model serves as a valuable tool for understanding demand dynamics, offering insights into market-specific patterns and facilitating informed decision-making in new markets.


## General Information
BoomBikes, a US bike-sharing provider, aims to boost post-lockdown revenue by understanding demand factors. To achieve this, they've enlisted a consulting company to analyze a dataset on daily bike demands. The company seeks to identify significant variables influencing bike demand and assess their predictive power. By leveraging meteorological surveys and lifestyle data, BoomBikes aims to develop a strategic business plan, differentiating itself and capitalizing on increased demand once the Covid-19 situation improves.

Datasets : Bike Sharing dataset

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
The ‘cnt’ variable can be represented as :
cnt = C1*season + C2*yr + C3*weathersit + C4*atemp + C5*casual + C6*registered, 
where the values of all the coefficients are : 
C1 = 2.429e-17
C2 = -3.816e-17
C3 = -2.914e-16
C4 = --3.331e-16
C5 = 0.3775
C6 = 0.7968 

From my analysis the model depends equally on categorical (yr, weathersit, season) and numeric (atemp, casual, registered) variables. None of the dependent variables have VIF factory more than 4 and all have P values < 0.5. As per the analysis we can see that the coefficients C1, C2, C3, C4 are very low. So the ‘cnt’ variable depends more strongly on ‘casual’ and ‘registered’ number of bikers. The factors such as ‘yr’, ‘weathersit’, ‘atemp’ affect ‘cnt’ negatively. The overal relation between the proposed variables and 'cnt' is linear.

## Technologies Used
### Technologies Used :
Python 3.11, Sklearn, Seaborn, Matplotlib, numpy, pandas, statsmodel

## Acknowledgements
Give credit here.
- This project was inspired by IIITB
- This project was based on EPGP course assignment.


## Contact
Created by Mostafijur28 - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->