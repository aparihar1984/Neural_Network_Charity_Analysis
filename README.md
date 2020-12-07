# Neural_Network_Charity_Analysis

## Overview of the Analysis

The purpose of this assignment/exercise was to use the features in the provided dataset to create a binary classifier that is capable of predicting whether applicants will be successful if funded by Alphabet Soup.  The purpose of this assignment/exercise was accomplished utilizing our knowledge of machine learning and neural networks.

## Results

Data Preprocessing:

The APPLICATION_TYPE and CLASSIFICATION columns/variables were the target variables for the model.  The SPECIAL_CONSIDERATIONS_Y and SPECIAL_CONSIDERATIONS_N were the features for the model.  The "EIN" and "NAME" columns/variables are neither targets nor features, and thus were removed from the input data.

[GitHub Site](https://github.com/aparihar1984/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity.ipynb)

Compiling, Training, and Evaluating the Model:

There were 111 neurons (hidden_nodes_layer1 = 80, hidden_nodes_layer2 = 30, units = 1), 3 layers (First Hidden Layer, Second Hidden Layer, and Output Layer), and  2 activation functions (relu, and sigmoid) in our model.

Were you able to achieve the target model performance? Yes, we did reach 75% accuracy.

What steps did you take to try and increase model performance?  We decreased the number of counts for both the replace_application (< 200) and the replace_class       (< 1500) functions. We also created a callback that saves the model's weights every 5 epochs.

[GitHub Site](https://github.com/aparihar1984/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimzation.ipynb)

[GitHub Site](https://github.com/aparihar1984/Neural_Network_Charity_Analysis/blob/main/AlphabetSoupCharity_Optimzation_Trial_2.ipynb)


## Summary

To summarize, in our initial test run prior to optimzation (AlphabetSoupCharity) we obtained an accuracy of 0.2620.  After our first optimzation 
(AlphabetSoupCharity_Optimzation), we obtained an accuracy of 0.9114.  After our second optimzation (AlphabetSoupCharity_Optimzation_Trial_2), we obtained an accuracy of 0.9992.

During the first optimzation, we only decreased the number of counts.  During the second optimzation, we created the callback that saves the model's weights every 5 epochs.  This resulted in an accuracy increase from 0.9114 to 0.9992.
