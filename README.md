# Predicting Customer Booking Behaviour 🛫🧑‍💼📊

This project involves training a machine learning model to predict if a customer will complete a booking. Our workflow includes data exploration, preprocessing, training the model, fine-tuning it, and visualizing its feature importances.

## Workflow 💻🔄

1. **Explore and prepare the dataset** 🧐📊: 
    We first load and explore our dataset to understand its columns and basic statistics. Then, we prepare our dataset for modelling by doing the following:
    - Converting the `flight_day` to numerical values.
    - One-hot encoding categorical variables like `sales_channel`, `trip_type`, `route`, and `booking_origin`.
    - Normalizing numerical features like `num_passengers`, `purchase_lead`, `length_of_stay`, `flight_hour`, `flight_duration`, and `flight_day`.
    - Adding an interaction feature `extra_services_sum` which is the sum of `wants_extra_baggage`, `wants_preferred_seat`, and `wants_in_flight_meals`.

2. **Train a Machine Learning Model** 🧠🔍:
    We use the RandomForest classifier to train our model. RandomForest is good for this purpose because it easily allows us to output information about how each variable within the model contributes to its predictive power.

3. **Hyperparameter Tuning** 🎛️🔧:
    We fine-tune the hyperparameters of our RandomForest model using GridSearchCV to find the best parameters that give the best performance.

4. **Evaluate Model** 📏🎯:
    After training our model, we evaluate it by conducting cross-validation and outputting evaluation metrics like accuracy, precision, recall, and F1 score. We also test our model on a test set and output the same metrics.

5. **Visualize Feature Importances** 📊🌟:
    We visualize the feature importances of our model to interpret how each variable contributed to the model. We also extract and visualize the top 10 most important features.

## Conclusion 🏁💡

This project shows how to leverage machine learning techniques to predict customer behaviour, in this case, the likelihood of completing a booking. This kind of prediction can be highly valuable to businesses in optimizing their marketing strategies and improving their services.

## Author

This project is created by Taha Khan. For any queries, feel free to contact me (tahak070@gmail.com).
