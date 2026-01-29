# spotify-popularity-regression
This repository implements a machine learning project dedicated to predicting the popularity of Spotify tracks on a scale of 0 to 100 based on their unique audio features and metadata. The analysis utilizes the "Spotify Tracks Dataset," a collection of approximately 114,000 songs spanning 125 distinct musical genres.


The modeling process focuses on learning a mapping from feature vectors—including perceptual attributes like danceability, energy, and loudness alongside metadata such as genre and explicit flags—to the true popularity score. Preprocessing involved removing non-predictive text identifiers and handling missing numerical values to ensure the data was suitable for regression analysis.



Two primary regression models were implemented and compared: a Random Forest Regression and a Multi-layer Perceptron (MLP) Neural Network. The Random Forest model used an ensemble of decision trees to capture nonlinear relationships, while the MLP utilized a three-layer architecture with 128, 64, and 32 neurons using the ReLU activation function. Performance was evaluated using Mean Squared Error (MSE) on a dataset split into 70% training, 15% validation, and 15% test sets.





The results demonstrated that the Random Forest model achieved superior predictive accuracy with an MSE of approximately 222, significantly outperforming the MLP's MSE of approximately 409. While the neural network offered theoretical flexibility, the ensemble method provided more robust and interpretable predictions on this specific dataset, which is influenced by noisy external factors like marketing and playlist placement.
