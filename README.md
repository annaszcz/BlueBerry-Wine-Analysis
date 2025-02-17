# BlueBerry-Wine-Analysis
Wine Quality Analytics
BlueBerry Winery, a start-up wine maker in Portugal, asked for help to determine the quality of wines based on their composition.
The goal of the project is to prepare the data to be fitted to a Machine Learning algorithm, analyse the data (taking into consideration the business questions), and present your findings.

# EDA 
The data I received was already clean, with consistent data types and no missing values. I merged the two datasets (red and white), added a new column to categorize wine quality (ranging from 3 to 9) into three simplified groups—low, medium, and high—and then proceeded with statistical analysis and visualizations.

# Machine Learning Modelling
I applied a Supervised Learning approach since the dataset consisted of measured features with associated labels. My goal was to train a model capable of assigning labels to new, unseen data in the future. To achieve this, I used a classification technique, which categorizes data into predefined classes. The labels used were quality categories (low, medium, high) and wine type (red, white).

Machine Learning Models Used:
  Logistic Regression: Used to determine the best-fitting relationship between the dependent variable (the discrete quality or type labels) and the independent variables.
  K-Nearest Neighbors (KNN): A simple algorithm that stores available cases and classifies new data based on a similarity measure.
  Decision Tree: Continuously splits data based on specific parameters. The model consists of decision nodes, where data is split, and leaves, which represent final classification    outcomes.
  Random Forest: Constructs multiple decision trees during training and outputs the class that is the majority vote of all trees.

Step-by-Step Approach:
  Feature Selection: Confusion Matrix plus ANOVA Test.
  Identified relevant variables while discarding irrelevant inputs.
  Simplified models improve interpretability and often lead to better performance.
  Avoided overfitting (excessively complex models) while ensuring the model had enough learning capability.
  Model Training & Prediction.
  Fitted the models to the dataset and generated predictions.
  Accuracy Evaluation:
      Confusion Matrix: A table to visualize the algorithm’s performance.
      Classification Report
      Precision: The ratio of true positives (TP) to total predicted positives (TP + FP).
      Recall: The ratio of true positives (TP) to actual positives (TP + FN).
      F1-score: A weighted harmonic mean of precision and recall, where a score of 1 is the best and 0 is the worst.
      Support: The number of occurrences of each class in y_test.
      Cross-Validation - used to assess the model’s generalizability by splitting the dataset into multiple subsets.
Implemented k-fold cross-validation, where k (CV parameter) defines the number of groups the dataset is divided into.
