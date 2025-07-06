# Principal-Component-Analysis
This encompases the development of model that addresses referrals at a cancer center.
The dataset for this analysis is from Cancerer Dataset downloaded from sklearn.datasets .
The dataset has 32 columns, the first column is the the ID while the second column is the diagnosis that consist of M for malignant and B for benign.
Principal Component Analysis is the technique that has been identified as the prefered for the task
In other to demonstrate how essential variables can be acquired from the dataset from the Cancer center, a python script was created that shows PCA performance on the dataset.
Preprocessing involves separating the features and the labels,missing and invalid data are taken care of  and well as standardization of the of the numerical features.
Scikit-learn's PCA is applied to redduce dimensionality and compute explained variance ratios.
The scatter plot shows the data points in the PC1-PC2 plane with the samples from both the malignant and benign forming distinct clusters and that indicates that PCA captures meaningful variance related to diagnosis
While the scree plot tried to show the explain variance ratio, this implies that the first few components(PC1 and PC2) explain a significant potion of the variance

PCA reduces the 30-column feature to a smaller components that capture the most variance. 

# Reduce the Dataset into 2 PCA Dataset
The output in the case involves a reduced_cancer_dataset csv file. The dataset includes columns such as the ID,PC1 and PC2.
The visualization include a scatter plot with 2 distinct clusters for M and B
This reduced dataset is suitable for further analysis as well as visualization. This capures the most significant variance in just 2 dimensions. 
# Implement logistic regression for prediction
To implement logistic regression for prediction using the reduced_cancer_dataset, a python was created  and that will be used in the training of the logistic regression modelon the 2 PCA components to predict the diagnosis(m=malignan,B=benign)
The data is split into 2, training and testing sets and a logistic regression model is trained using scikit-learn to predict the diagnosis
The visualization involves a decision boundry in the PC1-PC2 plane separating the malignant and benign classes.
The logistic regression model leverages the 2 PCA components in the effective prediction of cancer diagnosis and the visualization provides better interpretation of the models behavior.
