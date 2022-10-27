### -----------------------------------------------------------------------------------------------------
# Decision Trees - Spine Surgery
### -----------------------------------------------------------------------------------------------------
### Decision Trees:
- an **algorithm**:
    - based on **Supervised Learning**
    - to solve **Regression and Classification**
    - where machines **learn with supervision**
    - **input data are labeled** and **expected output data is known**
    - with key **objective**:
        - **to predict (classify) a categorical (qualitative) dependent output value (y)** based on **independent input variable(s) (x)** -> for **Classification problems**
        - **to predict a continuous (quantitative) numeric dependent output value (y)** based on **independent input variable(s) (x)** -> for **Regression problems**
    - by **choosing the feature that best split the data** we try:
        - **to predict the class that is the mode of the classes of the individual trees**
        - **to predict mean prediction of the individual trees**
- **Regression and Classification** are a **predictive modeling techniques**
- **Structure of a Decision Trees**:
  - Nodes -> split for the value of a certain features
  - Edges -> outcome of a split to next node
  - Root -> node that performs the first split
  - Leaves -> terminal nodes that predict the outcome                
- **Choosing the best split** in order to pick **which feature to split on**:
  - **Information Gain** -> if there is a single yes/no question that accurately predicts the outputs 99% of the time, then that question allows us to “gain” a lot of information about data
  - **Entropy** -> measure how much information we gain (a measure of uncertainty associated with data)    
- Behave with **“if this, then that”** condition                   
- **Not** to be used **for larger datasets**

### -------------------------------------------------------------------------------------------------------
### Project Objective: Predicting if spine surgery was successful
Create a model that allows to put in a few features of children who have had corrective spine surgery due to Kyphosis and returns back a prediction (classification) if the corrective spine surgery was successful. Information about the children who have had corrective spine surgery is in the dataset 'Kyphosis_Data.csv'. The Kyphosis dataset has 81 rows and 4 columns. 

The Kyphosis dataset contains the following columns:
- **Kyphosis** - present or absent after operation
- **Age** - age of children at time of operation (in months)
- **Number** - number of vertebrae involved in the operation
- **Start** - number of first (top-most) vertebrae that was operated on

**Source**: John M. Chambers and Trevor J. Hastie eds. (1992) Statistical Models in S, Wadsworth and Brooks/Cole, Pacific Grove, CA.

### -------------------------------------------------------------------------------------------------------
### Table of Contents:
1. File Descriptions
2. Technologies Used
3. Structure of Notebook
4. Executive Summary

#### 1. File Descriptions
- Decision Trees - Spine_Surgery.ipynb
- Kyphosis_Data.csv
- README.md

#### 2. Technologies Used
- Python
- Pandas
- Numpy
- Matplotlib
- Seaborn
- Scikit-Learn

#### 3. Structure of Notebook
1. Import the Libraries
2. Load the Data
3. Exploratory Data Analysis
    - 3.1 Check out the Data
    - 3.2 Data Visualization
4. Data Preprocessing and Feature Engineering
    - 4.1 Identify the variables
    - 4.2 Dealing with Missing values
    - 4.3 Dealing with the Non-numerical features
5. Train and Test the Decision Tree Classifier model
    - 5.1 Split the columns
    - 5.2 Split the data into Training dataset and Testing dataset
    - 5.3 Create the Decision Tree Classifier model
    - 5.4 Train / fit Decision Tree Classifier model
    - 5.5 Predictions from the model on Testing data
    - 5.6 Evaluate the model on Testing data
      - 5.6.1 Classification report
      - 5.6.2 Confusion matrix
    - 5.7 Feature importance
    - 5.8 Tree visualization
    - 5.9 GridSearchCV
      - 5.9.1 Create the Grid of parameters
      - 5.9.2 Create the GridSearchCV model (Re-create the Decision Tree Classifier model)
      - 5.9.3 Train / fit the GridSearchCV model (Re-train / Re-fit the Decision Tree Classifier model)
      - 5.9.4 Predictions from the GridSearchCV model (Re-predictions from the Decision Tree Classifier model) on Testing data
      - 5.9.5 Evaluate the GridSearchCV model (Re-evaluate the Decision Tree Classifier model) on Testing data
        - 1. Classification report
        - 2. Confusion matrix

#### 4. Executive Summary
TBA
