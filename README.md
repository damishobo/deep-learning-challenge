# deep-learning-challenge

## Overview of the analysis: 
- The purpose of my analysis was to be able to predict with more accuracy on the deep learning model whether applicants will be successful if funded by Alphabet Soup

## Results
- Data Preprocessing: The variable 'IS_SUCCESSFUL' was the target for my model while the rest of the variables were the features for my model as shown in the image below. In addition, 'EIN' and 'NAME' were variables removed from the input data because they are neither targets nor features
<img width="681" alt="Screenshot 2023-05-17 at 23 48 26" src="https://github.com/damishobo/deep-learning-challenge/assets/119973334/4f83e2f4-a4a6-4519-919f-ee02bfb20eab">

- Compiling, Training, and Evaluating the Model: I selected three layers for both the initial neural network model and when optimizing said model to increase the capacity of the model and make it more efficient. I also used two different activation functions ('relu' and 'sigmoid'). All this can be seen in the first image below. I was able to achieve the target model performance which was higher than 75% and got a model accuracy score of 0.78950434923172. This can be seen in the second image below.
<img width="1012" alt="Screenshot 2023-05-17 at 23 59 41" src="https://github.com/damishobo/deep-learning-challenge/assets/119973334/941bc59e-391a-460c-96f3-2c56f89e2bde">
<img width="701" alt="Screenshot 2023-05-18 at 00 09 19" src="https://github.com/damishobo/deep-learning-challenge/assets/119973334/3cc04c2f-d8b2-414b-8a65-4e0096e55b13">

- Continuation of Compiling, Training, and Evaluating the Model: In order to increase model performance, I firstly only dropped the 'EIN' column from the initial dataframe and left the 'NAME', something I did not do before beginning the optimization of the model. I then looked at the 'NAME' value counts for binning, chose a cutoff value and created a list of name types to be replaced in my dataframe. After this step that I added when optimizing my model, I repeated the same steps from my previous model but made sure that the columns I was converting from categorical data to numeric with 'pd.get_dummies' were object data types. The next step I made to increase model performance was to change the number of input features from 43 to 398 so that the high number of columns gotten from converting the categorical data to numeric would fit in my model. All these steps aided me in improving the performance of my model.

## Summary
- The overall results of my the deep learning model are that I can predict as accurately as asked (over 75%) whether applicants will be successful if funded by Alphabet Soup.
