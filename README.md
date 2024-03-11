# deep-learning-challenge

# Report on the Neural Network Model for Alphabet Soup

## Overview of the Analysis:
The purpose of this analysis is to develop a deep learning model using TensorFlow to predict the success of funding applications for Alphabet Soup, a non-profit organization. The model aims to classify whether funding applicants will be successful based on various input features provided in the dataset.

## Results:

### Data Preprocessing:
- **Target Variable:** The target variable for my model is `IS_SUCCESSFUL`, which indicates whether a funding application was successful (1) or not (0).
- **Features:** The features for my model include all columns except for `IS_SUCCESSFUL`, `EIN`, and `NAME`.
- **Variables to Remove:** I removed the non-beneficial columns `EIN` and `NAME` as they do not contribute to the model's predictive power.

### Compiling, Training, and Evaluating the Model:
- **Neurons, Layers, and Activation Functions:** 
  - I selected a neural network architecture with three hidden layers consisting of 256, 128, and 64 neurons, respectively.
  - I used ReLU activation functions for all hidden layers and a sigmoid activation function for the output layer since it is a binary classification problem.
- **Target Model Performance:**
  - Despite several attempts to optimize the model by adjusting the architecture, training parameters, and preprocessing techniques, I was unable to achieve the target model performance of 75% accuracy.
- **Steps Taken to Increase Model Performance:**
  - I increased the complexity of the neural network architecture by adding more neurons and layers to capture intricate patterns in the data.
  - Dropout regularization was employed to prevent overfitting by randomly dropping out nodes during training.
  - I adjusted hyperparameters such as the number of epochs and the batch size to find the optimal balance between underfitting and overfitting.

### Summary:
The deep learning model achieved an accuracy of approximately 72.48%, which falls short of the target performance threshold. Despite my efforts to optimize the model, it appears that the dataset may not contain enough discernible patterns for the neural network to learn effectively. 

## Recommendation:
Considering the limitations of the neural network model, an alternative approach using ensemble learning techniques, such as Random Forest or Gradient Boosting, could potentially yield better results. Ensemble methods combine multiple models to improve predictive performance and are less susceptible to overfitting. Additionally, incorporating feature engineering techniques and exploring more sophisticated preprocessing methods may enhance the model's ability to capture relevant information from the data. 
# References
IRS. Tax Exempt Organization Search Bulk Data Downloads. https://www.irs.gov/
