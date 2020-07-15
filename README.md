# Artificial_Neural_Network

## Breast Cancer Prediction using SVM with PCA Feature Selection in a Pipeline

The goal is to classify whether the breast cancer is benign or malignant by applying hyper
parameter selection. To achieve this I have used machine learning classification method:
Support Vector Machine (SVM) to fit a function that can predict the discrete class of new
input.

Keywords: Breast Cancer, Support Vector Machine, PCA, Scaling, Kernel tricks, Pipeline,
GridSearchCV, Cross-Validation

Methodology:

SVM is a supervised machine learning classification technique that divides the datasets into
classes using convenient maximal margin hyperplane (the optimized decision boundary).
This algorithm performs margin maximization by creating maximum gap between different
classes. To evaluate the performance of this algorithm I calculated its accuracy.

To prevent the problem of overfitting and outliers and applied different scaling methods
(Standard, Robust and MinMax) and testing different Kernel functions in order to find the
widest road between different samples (Linear and RBF).

After scaling the data, I applied Principal Component Analysis (PCA) to improve the
accuracy by decreasing the number of parameters (as there are 30 features in total)
Finally, with the use of GridSearchCV, I built a pipeline helps to enforced desired order of
application steps which eventually we facilitate the reproducibility and create the workflow.
Results: The obtained accuracy is 97%, by choosing 2 principal components, with parameters
‘C=1’ and ‘Gamma=0.001’ for SVM with Linear kernel by cross validating 6 folders. 
