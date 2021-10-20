# Neural_Network_Charity_Analysis

## Purpose

By utilizing neural networks, an attempt was made to create a classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup. The database contained information on over 34,000 organizations that have received funding from the charity. 

## Results 

### Data Preprocessing

* Target variable for the data set was binary IS_SUCCESSFUL—Was the money used effectively
* Features of the dataset inluded; Application Type, Affiliation, Classification, Use_Case, Organization, Status, Income_AMT, Special_Considerations, and Ask_AMT
* variables that were not relevant and dropped from the data set included EIN and Name 

### Compiling, Training, and Evaluation the Model

Initially, the following parameters were chosen for our model:
* 110 initital nuerons 
* spread over 2 hidden layers (80 in the first, 30 in the second) chosen as it is recommended the inititla hidden layer contain twice as many nuerons as input variables, and the second hidden layer having half as many as the first 
* The activation function ReLU was used for both hidden layers 
* Sigmoid was used for the ouput layers as it was the ouput was a binary choice 

Unfortunately, we were unable to achieve the 75% accuracy target model performance, even after optimizations. These optimizations included:
* Increasing the number of hidden layers from 2 to 4
* increasing the nuerons per hidden layer 
* changing the activation function to tanh and LeakyReLU
* Eliminating variables from the dataset that we felt might be causing noise, such as STATUS, and many of the "Other" classifications from the bucketed variables 

### Summary 

As stated, the nueral network was unable to achieve the required 75% accuracy, even after optimization. Overall, it seems the model underfit the data available. A possible alternative model that could be employed would be the random forest model, which might be able to better identified which features were most important to the taarget outcome. 
* 
