Airline Satisfaction Prediction

This project predicts airline passenger satisfaction using machine learning. It handles both numerical and categorical features, applying One-Hot Encoding to categorical data and training a Random Forest Regressor.

Model Fitting

Load dataset and drop missing values.

Separate features (X) and target (y = satisfaction).

Split data into training and test sets (train_test_split).

Preprocess data with ColumnTransformer:

Pass numerical features as-is.

One-Hot Encode categorical features.

Build a pipeline: Preprocessor → Random Forest Regressor.

Train the model with model.fit(X_train, y_train).

Prediction

Prepare new data with all columns used in training.

Make predictions using model.predict(new_data).

Example output: Predicted satisfaction scores (continuous values).

Note: Missing columns in new data will raise an error. Ensure all features from the training set are present.
