Party Guest Classifier
This project uses machine learning algorithms to classify UiB students as either "ok" or "not ok" party guests based on categorical features such as gender, age, faculty, hobbies, music preferences, and whether they dance at parties.

Algorithms Used:
1. K-Nearest Neighbors (KNN): The dataset is one-hot encoded using get_dummies(), and the KNN algorithm is applied with different k values (e.g., 5). The model predicts whether a student is an "ok guest" by comparing features with neighboring data points. Accuracy, precision, and confusion matrix are used to evaluate performance.
2. Decision Tree: Two decision tree classifiers are implemented with different criteria (Gini and Entropy). The same one-hot encoded data is used to train and test the decision trees, and the models are evaluated using accuracy and confusion matrices.
3. Logistic Regression: Logistic regression is applied with and without regularization (penalty). The data is encoded with drop_first=True to avoid multicollinearity. Both versions of the model are evaluated on accuracy and precision for the test data.
	
Evaluation:
For each algorithm, the dataset is split into training (80%) and testing (20%) sets using train_test_split(). The models are evaluated based on their accuracy, precision, and confusion matrices. This comparison helps determine the best model for predicting which students will be "ok" guests at a party.

