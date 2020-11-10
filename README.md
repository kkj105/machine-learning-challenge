# machine-learning-challenge
Create a README that reports a comparison of each model's performance as well as a summary about your findings and any assumptions you can make based on your model (is your model good enough to predict new exoplanets? Why or why not? What would make your model be better at predicting new exoplanets?).

Modeling this data held consistently steady. Neither model varied greatly from the other, however, model 2 was chosen because when creating a Random Forest Classifier, more n_estimators were selected in order to create more trees in the forest. 

Both models were found to have training data with a score of 84%, and testing data with a score of 86%. The most important features (with the heaviest weight in this modeling) were found to be koi_fpflag_ss and koi_disposition.

After using GridSearch and tuning the parameters, the best parameter for model_2 was found to be C:100, gamma: 0.0001 and a best score of 88%. Based upon predictions of the test data, a Confirmed classification was correct 99% of the time, False Positive 82%, and Candidate 77%. With these findings, model_2 is accurate enough to be used to predict new exoplantets. The amount of times the model incorrectly confirms a new exoplanet are far less than the amount that it correctly confirms one. Even though both models performed so similarly, an opportunity to add additional data to the model would continue to improve how the model selects confirmed exoplanets versus not dispositioned. 
