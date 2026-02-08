PCA – Dimensionality Reduction 

Report 

 

Objective: 


The objective of this task is to reduce the dimensionality of image data using Principal Component Analysis (PCA) while preserving maximum information. The goal is to transform high-dimensional digit image features into a lower-dimensional space, analyze explained variance, and evaluate model performance before and after dimensionality reduction. 


Approach: 


I have load the digits dataset using sklear.datasets, and image data was converted into numerical feature vectors. I have applied Feature scaling using StandardScaler to ensure equal contribution of all features. PCA was then applied with multiple component values (2, 10, 30, 50) to observe variance retention. Then I calculated the explained variance ratio and cumulative variance to identify the optimal number of components. The dataset was transformed into a reduced feature space using the selected component count. Logistic Regression was trained separately on the original dataset and PCA-reduced dataset. Model performance was evaluated using accuracy comparison. Finally, the dataset was visualized in 2D space using PCA with two principal components. 

Results

Dimensionality reduction successfully compressed the dataset while retaining most of the important information. The cumulative variance plot helped identify an optimal number of components for effective representation. The classification accuracy using PCA-reduced data remained close to the accuracy of the original dataset, showing that PCA preserved essential patterns. The 2D visualization clearly showed clustering of digit classes in reduced space.

Reduced shape: (1797, 30)

Accuracy (Original Data): 0.9722222222222222

Accuracy (PCA Reduced Data): 0.9611111111111111


Conclusion: 

PCA proved effective in reducing data dimensionality while maintaining meaningful structure in the dataset. The reduced dataset required less computational power and still produced comparable classification performance. This demonstrates that PCA is a powerful preprocessing technique for machine learning tasks involving high-dimensional data. The experiment confirms that dimensionality reduction can improve efficiency without significantly affecting model accuracy. 
