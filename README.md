# KNN Classifier Model

### Objective

A project to build a KNN classifier to find whether a patient would have diabetes or not.

### Feature and the target varaible

X- The feature variables :
- Pregnancies
- Glucose
- BloodPressure
- SkinThickness
- Insulin
- BMI
- DiabetesPedigreeFunction
- Age

y - Target variable
- Outcome

### Determining n_neighbours 

- From a range of 1 to 9 , the n_neighbors are selected passing them through a for loop to test each case and then the training accuracy and testing accuracy graph is plotted along with Number of neighbors with respective to accuracy. Vizualising the graph neighbor having the value of 4 has a greater testing accuracy and when fitted to the model it gives 72.7% of best score.


### Accuracy prediction
- Classification report 
- Confusion matrix : True positive = 90     True negative = 10
                     False positive = 32    False negative = 22

### Plotting the ROC Curve and predicting the AUC score
- Plotting the true positive rates with respective to false positive rates for different possible cut points of a diagonstic point 
- Finding the area under ROC curve and thus predicting the score which is equal to 0.698%

### Passing a new data to predict whether a patient has diabetes or not

 Two new data's were passed for prediction and the model predicted that patient 1 has diabetes and patient 2 has no diabetes .
 
### Hyper parameter turing - Grid Search CV
 
 - Another method to determine n_neighbors is to tune the hyper parameters to choose the best best value. Grid search cv method is applied to the model to determine the best value for K nearest neighbor from the range of 1 to 50 . The best score with n_neighbors = 14 gives 75.78% accuracy.

