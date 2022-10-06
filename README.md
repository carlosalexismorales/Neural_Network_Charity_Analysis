# Neural_Network_Charity_Analysis


## Project Overview

Alphabet Soup, a non-profit foundation, needs help vetting potiental recipients for their donations. We are tasked to predict which are worth donating to and which are too high risk. To help us accomplish this, we are creating a mathematical data driven solution that can do this accurately. A deep learning neural network is designed and trained to evaluate all types of input data and produce a clear decision making result using the Python TensorFlow library. This model will ultimately help Alphabet Soup determine which organizations should receive donations. 


## Challenge Overview

1. Preprocessing Data for a Neural Network Model
2. Compile, Train, and Evaluate the Model
3. Optimize the Model

## Results


### Preprocessing the Data

The images below contain the code for data preprocessing 

- The EIN, NAME, STATUS, and SPECIAL_CONSIDERATIONS were neither targets nor features and were removed from the data
- The IS_SUCCESSFUL column was considered the target for the model 
- The APPLICATION_TYPE, AFFILIATION, CLASSIFICATION, USE_CASE, ORGANIZATION, INCOME_AMT, and ASK_AMT columns are considered to be the features for the model



<img width="1011" alt="Screen Shot 2022-10-05 at 6 18 29 PM" src="https://user-images.githubusercontent.com/102444078/194192603-ae80beee-eb55-4a15-a951-75aa1e3de588.png">




<img width="1006" alt="Screen Shot 2022-10-05 at 6 19 21 PM" src="https://user-images.githubusercontent.com/102444078/194192709-2995de4b-d506-42bd-b271-f5ba5885d657.png">




<img width="1010" alt="Screen Shot 2022-10-05 at 6 19 43 PM" src="https://user-images.githubusercontent.com/102444078/194192762-244d2b25-8a8b-46d2-9ae5-ebfa00dc0026.png">




### Compiling, Training, and Evaluating the Model


The images below contain the code for designing the model 


- 120 neurons with a sigmoid function for the first hidden layer 
- 50 nuerons with a ReLU function for the second hidden layer
- 18 neurons with ReLU for the third hidden layer 
- Sigmoid function for the outer layer  
- I chose to change the activation function to sigmoid since after running the code multiple times, its performance was going on an upward trend. 
- The model achieved an accuracy of 71% and was not able to meet the goal of 75%, however, it did perform better than my first model which had an accuracy of 70%
- The model's performance was increased and changed by eliminating columns and creating more bins for rare occurances in columns, decreasing the number of values in some bins, adding more neurons and hidden layers, and using a differnet activation function


<img width="1004" alt="Screen Shot 2022-10-05 at 6 22 45 PM" src="https://user-images.githubusercontent.com/102444078/194193050-c0ee2d5e-9091-46ba-abb8-77c39d339f82.png">




<img width="1006" alt="Screen Shot 2022-10-05 at 6 23 09 PM" src="https://user-images.githubusercontent.com/102444078/194193084-9a0582f9-f51e-4575-9325-7c2b262241c0.png">






<img width="1143" alt="Screen Shot 2022-10-05 at 6 23 32 PM" src="https://user-images.githubusercontent.com/102444078/194193128-33ad711c-6ed8-4b39-b671-4c3278c3151b.png">







## Summary

The optimized AlphabetSoup neural network performed better than the first version. Although the improvement in performance was minimal, this is a step in the right direction towards creating one that can achieve target performance. The loss metric, for example, fell from 0.93 to 0.81, meaning that there is less model error, which can help make better decisions for Alphabet Soup. We can continue to modify the model by removing more superfluous columns, adding more neurons and hidden layers, and using different activation functions. 

One recommendation to an alternative to solve this could be using a Random Forest model. A random forest is a supervised machine learning algorithm that is constructed from decision tree algorithms. The model builds smaller decision trees until it generates a classified output. 


