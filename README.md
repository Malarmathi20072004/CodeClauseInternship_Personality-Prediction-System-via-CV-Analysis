# CodeClauseInternship_Personality-Prediction-System-via-CV-Analysis

The project aims to predict personality traits based on the analysis of an individual's Curriculum Vitae (CV). The system utilizes a machine learning model, specifically a logistic regression model, trained on a dataset containing information associated with personality traits.

Data Set Details

Openness: Curiosity, imagination, and appreciation for new experiences.

Conscientiousness: Reliability, organization, and thoroughness in tasks.

Extraversion: Sociability, assertiveness, and energy in social situations.

Agreeableness: Warmth, friendliness, and cooperation towards others.

Neuroticism: Emotional stability, or conversely, susceptibility to negative emotions.


Work Flow

Training the Model (train_model class):
Reads a CSV file ('training_dataset.csv') containing training data.
Converts gender labels to numeric values.
Extracts features and labels from the dataset.
Uses a logistic regression model (linear_model.LogisticRegression) to train the model.

Testing the Model (test method):
Takes a list of test data as input.
Predicts the personality using the trained logistic regression model.
Returns the predicted personality.

Data Type Checking (check_type function):
Checks the type of data and converts it to a desired format.
Handles cases for strings, lists, tuples, and other data types.

Prediction Result Display (prediction_result function):
Closes the previous Tkinter window.
Calls the test method to get the predicted personality.
Parses information from the resume using pyresparser.
Displays the entered data, predicted personality, and parsed resume information in the console.
Creates a new Tkinter window displaying the predicted personality along with parsed resume information and personality definitions.

Personality Prediction Interface (perdict_person function):
Opens a new Tkinter window for personality prediction.
Takes user inputs for applicant name, age, gender, CV file, and personality traits.
Uses radio buttons for gender selection.
Calls OpenFile to choose a file for the CV.
Validates and processes the user inputs.
Displays the predicted personality, applicant name, age, and parsed resume information in a new full-screen Tkinter window.

File Selection (OpenFile function):
Opens a file dialog to choose a resume file.
Updates the button text with the selected file's name.

Main Execution:
Creates an instance of the train_model class (model) and trains the model.
Initializes the main Tkinter window for the application.
Provides a button to trigger the personality prediction interface.


Conclusion

he Personality Prediction System via CV Analysis project merges machine learning, CV parsing, and user interface design to provide a tool for predicting personality traits based on the content of a CV. The project strives to offer a valuable and accessible resource for both users seeking personality insights and developers aiming to understand the intersection of machine learning and human attributes.



