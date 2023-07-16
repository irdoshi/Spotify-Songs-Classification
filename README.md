# Spotify-Songs-Classification

This project aims to classify Spotify tracks into different genres using machine learning algorithms, specifically Decision Tree and Random Forest. The dataset used is the Spotify Tracks Dataset obtained from Kaggle, which contains various audio features of tracks across different genres.


The following steps were performed in this project:

- Data Collection: The Spotify Tracks Dataset was collected and cleaned using the Spotify Web API and Python.

- Data Preprocessing: The dataset was inspected for missing values and duplicates, which were then removed. The "Unnamed: 0" column, which appeared to be an index column, was dropped. The "explicit" feature was converted from a boolean to a float representation.

- Model Training and Evaluation:

- - Decision Tree: The initial classification was performed using a Decision Tree classifier. The dataset was split into training and testing sets, and the Decision Tree model was trained on the training set. The accuracy, precision, recall, and F1-score of the model were evaluated on the testing set.

- - Random Forest: To potentially improve the classification accuracy, a Random Forest classifier was also used. The dataset was split into training and testing sets, and the Random Forest model was trained on the training set. The accuracy, precision, recall, and F1-score of the model were evaluated on the testing set.

- - Feature Selection: To identify the most informative features, a correlation analysis and feature importance ranking were performed. The top 10 features were selected, and a Decision Tree model was trained and evaluated using only those features.

- - Scaling: The features were scaled using StandardScaler and RobustScaler to assess their impact on the classification performance. Decision Tree models were trained and evaluated on the scaled features.

- - Pruning: Pruning was applied to the Decision Tree model by adjusting the minimum samples split, maximum depth, and maximum features parameters. The pruned model was trained and evaluated on the testing set.

- - Data Type Transformation: The data type of the "explicit" feature was transformed to float. The Decision Tree model was trained and evaluated on the transformed dataset.

- - Model Performance Comparison: The accuracies, precisions, and recalls of various models were compared using visualizations. The models compared include Decision Tree, Top 10 Features, Scaled Decision Tree, Robust Scaled Decision Tree, Pruned Decision Tree, Transformed Decision Tree, Random Forest Classifier, and Transformed Random Forest.
