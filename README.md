# Prediction of Demand for Bike Sharing
> A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. A bike sharing owned company wishes to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the market.


## Table of Contents
* [General Information](#general-information)
* [Tools and Technologies Used](#tools-and-technologies-used)
* [Conclusions](#conclusions)
* [Contact](#contact)


## General Information
- Project Overview: A bike sharing owned company wishes to understand the factors on which the demand for these shared bikes depends.
- Background: A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Specifically, they want to understand the factors affecting the demand for these shared bikes in the market.
- Business Problem: Identify the variables are significant in predicting the demand for shared bikes, to create a linear model that quantitatively relates bike demands with variables provided and to know the accuracy of the model, i.e. how well these variables can predict bike demands
- Dataset: Bike Sharing data from 2018 and 2019.


## Tools and Technologies Used
To run this project, you need to have Anaconda Jupyter Notebook and Python installed
- pandas
- numpy
- matplotlib
- statsmodel
- sklearn


## Conclusions
### Key Insights from model:
- R-Squared value on train data is 75.2%, which indicates the variability in bike demand (cnt) is explained by the model. This is a good fit, showing that the selected variables describe the bike demand reasonably well.
- All the assumptions are validated such as error terms are normally distributed and are independent of each other.
- R-Squared value on test data is 73.5%, and hence it concludes that, this model has a good understanding of training data and it can predict the test data properly.
- The equation of our best fitted line is  cnt=0.2801+0.2473×2019_yr−0.1770×windspeed+0.2573×summer+0.3162×fall+0.2268×winter−0.0857×mist−0.2877×light_snow

### Significant features in Prediction
- 2019_yr: This variable indicates whether the data point is from the year 2019. It has a p-value of 0.000, suggesting strong significance. The positive coefficient (0.2473) indicates that bike demand increased in 2019.
- windspeed: The negative coefficient (-0.1770) with a p-value of 0.000 indicates that higher windspeed decreases bike demand.
- summer, fall, winter (season): These are dummy variables representing different seasons. All have significant p-values (0.000), indicating their importance in predicting bike demand. Positive coefficients for these variables suggest higher bike demand in these seasons compared to the omitted season (likely spring).
- mist: This variable represents weather conditions with mist, and its negative coefficient (-0.0857) indicates lower bike demand on misty days.
- light_snow: The negative coefficient (-0.2877) with a p-value of 0.000 shows that light snow significantly reduces bike demand.


## Contact
Created by [https://github.com/udaykiranpujaari72] - feel free to contact me!
