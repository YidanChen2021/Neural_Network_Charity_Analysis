# Neural_Network_Charity_Analysis  
## Overview of the analysis  
Alphabet Soup is a Nonprofit Networking company thats dedicated in funding and helping other orgazitions protect environment, improve people's wellbeing and unify the world. This project is brought out through Neural Networks and Machine Learning to analyze the datasets of 34,000 organizations that have received fund from Alphabet Soup, and help to predict if the funding impact will be successful. 

## Results  
The project was initated with Data preprocessing: 
* What variable(s) are considered the target(s) for your model:'IS_SUCCESSFUL'
* What variable(s) are considered to be the features for your model:  
  [APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, ORGANIZATION, STATUS, INCOME_AMT, SPECIAL_CONSIDERATIONS, ASK_AMT]                  
* What variable(s) are neither targets nor features, and should be removed from the input data:  
  Variables [EIN, NAME] are neither targets nor features. They should removed from the data.  
  
The second step was to complie, train and evaluate the model. 
* There were 2 hidden layers and 1 output layers in my neural network model.
  * Hidden Layer 1: 80 neurons, activation function: relu  
  * Hidden Layer 2: 30 neurons, activation function: relu  

* The model performed with 70.18% accuracy, which is lower than the target of 75%.  
* The following steps were taken to increase the model performance:  
  * Removing Features: received 54.20% accuracy and 0.705 in loss.
![Attempt 1](https://user-images.githubusercontent.com/93500353/159197980-32e101e8-534d-4a70-a06b-d21c76e998cf.png)  
  * Adding more neurons to a hidden layer and more hidden layers: increased neurons in layer 1 to and 50 to layer 2, added layer 3 with 20 neurons. Received 53.33% and 0.746 in loss.  
![Attempt 2](https://user-images.githubusercontent.com/93500353/159198481-9509fc50-1419-40f8-b951-bd1f1687f749.png)  
  * Using different activation functions to the output layer: changed the activation function to 'tanh' in output layer, received 52.80% in accuracy and 1.38 in loss.
![Attempt 3](https://user-images.githubusercontent.com/93500353/159198650-c194ccbb-49b7-45d5-9f2c-c6526a8702b0.png)  

## Summary  
The neural network model hasn't reached the target accuracy rate. With the optimization attempts, the accuracy didn't increase as expected. Indeed, it dropped compared to the first model. Recommend to try it with Random Forest method. 

