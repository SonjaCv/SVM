# Support vector machines

The code in index.txt creates an SVM model and predicts new unlabeled data using functionalities implemented in the LIBSVM library
The file trainingData.txt contains both the class labels and the data features. The first column is the class label and the rest of the columns are data examples organized in the following pattern: column number: feature value; 
libsvmread (LIBSVM) reads the dataset and saves the class labels in label_vector and the feature values in instance_matrix.

With svmtrain(LIBSVM) an SVM model is created. -t 2 in the settings means use the radial basis function as a kernel. This is built in functionality of LIBSVM. 

After testing and checking the accuracy we predict new labels for test data with the optimal model that was created.
The predicted values are saved in SVM_pred.txt and are used for precision and recall calculations in PrecisionRecallCalculation.m file.
The code in ROC_Precision_Recall.ipynb creates the ROC graphs for precision and recall.
