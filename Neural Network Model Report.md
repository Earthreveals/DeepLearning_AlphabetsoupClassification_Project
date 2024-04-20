**Report on the Neural Network Model for Alphabet Soup

***Overview of the Analysis

The purpose of this analysis was to create a deep learning model that can accurately predict the success of funding applications for Alphabet Soup, a philanthropic organization. By using historical data, the model aims to discern patterns and characteristics of applications that lead to successful funding outcomes, enabling Alphabet Soup to make more informed decisions on future applications.

***Results

**Data Preprocessing

Target Variable(s): The target for the model is the 'IS_SUCCESSFUL' column, which indicates whether the funding application was successful (1) or not (0).
Feature Variables: The features for the model include various descriptive attributes of each application, such as 'APPLICATION_TYPE', 'AFFILIATION', 'CLASSIFICATION', 'USE_CASE', 'ORGANIZATION', 'STATUS', 'INCOME_AMT', 'SPECIAL_CONSIDERATIONS', and 'ASK_AMT'.

**Irrelevant Variables: 

The 'EIN' (Employer Identification Number) and 'NAME' columns were removed from the input data. These identifiers are unique to each application and do not contribute to the model's ability to generalize to new applications.

**Compiling, Training, and Evaluating the Model

***Neurons, Layers, and Activation Functions:

The model was designed with two hidden layers.
The first hidden layer had 80 neurons, and the second had 30 neurons.
The 'relu' activation function was used for hidden layers to introduce non-linearity, and the 'sigmoid' function was used for the output layer to predict binary outcomes. Using the first model, we saw that it had an accuracy of 74 percent and loss of 53 percent. During training, there is a slight upward trend in accuracy, which suggests that the model is learning from the data.
The stable performance from training to testing suggests that there is no significant overfitting. The model seems to generalize well, which is a positive indicator of its reliability.

***Achieving Target Performance:

The target model performance was set as a high accuracy in correctly predicting the success of the applications. It is not specified here whether this target was achieved.

***Improving Model Performance:

We tried to optomize the model by adding another hidden layer and neurons. We added a third layer and adjusted the number of neurons in the first layer and second layer to 40 and 15. The new third layer had ten neurons. We saw that this optimization tactic producted a lower accuracy at 73.7 percent and loss of 53. The results were very similar even after the model performance used here.
Further optimization was done in the second model where a fourth layer with 10 neurons was used and the first three layers had, 90, 50 and 30 neurons. The neurons had been adjusted to minimize overfitting. This optimization provided same accuracy of 74 percent and practically the same loss at 52 percent. 
Additional data preprocessing steps such as feature selection, further feature engineering, or handling class imbalance, if present, could also be considered to get higher accuracy.
Regularization techniques to prevent overfitting, or increasing the amount of training data, could have been explored as well.

***Summary

The deep learning model constructed for Alphabet Soup was aimed at predicting the success of funding applications based on historical data. While the exact accuracy achieved by the model is around 74 percent, the model's architecture follows a standard approach for binary classification tasks.

***For future improvements or alternative approaches:

-A different model, such as a Random Forest or Gradient Boosting classifier, could be used to address this classification problem. These models can be more interpretable and might provide insights into feature importance.

-Ensemble methods, which combine multiple models to improve the final prediction, could also be considered.

-Given the binary nature of the classification problem, a logistic regression model could serve as a good baseline for performance comparison.

Ultimately, the choice of model would depend on the specific performance metrics Alphabet Soup is looking to optimize, such as accuracy, precision, recall, or F1 score, and the interpretability of the model's predictions. Regular updates to the model with new data and continuous testing are recommended to maintain and improve the prediction accuracy over time.






