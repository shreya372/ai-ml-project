Personalized Immediate Medicine Recommendation System


📋 Overview
This project is a Personalized Medical Recommendation System designed to assist users in understanding and managing their health. Leveraging machine learning, the system analyzes user-input symptoms to accurately predict potential diseases. Beyond simple prediction, it provides a comprehensive healthcare plan including descriptions, precautions, medications, diets, and workout routines.

🚀 Features
Symptom-Based Prediction: Accepts a list of symptoms from the user to predict the most likely disease.
Multi-Model Analysis: Evaluated against multiple algorithms (SVC, Random Forest, Gradient Boosting, KNN, Naive Bayes) to ensure high accuracy.

Comprehensive Recommendations:
Disease Description: Detailed explanation of the condition.
Precautions: Steps to take to prevent spreading or worsening.

Medications: Common drugs associated with the treatment.

Dietary Advice: Recommended foods to eat.

Workout Routines: Suggested physical activities.

🛠️ Tech Stack
Language: Python 3

Libraries:
pandas (Data manipulation) 
numpy (Numerical operations) 
sklearn (Machine Learning models and preprocessing) 
pickle (Model serialization) 

📂 Dataset & Prerequisites
The system relies on several datasets to function. Ensure the following files are present in your datasets/ directory:

Training.csv (Used for training the model)

symtoms_df.csv

precautions_df.csv

workout_df.csv

description.csv

medications.csv

diets.csv

The training data consists of 4,920 records with 133 columns representing various symptoms.


🧠 Model Training & Performance
The system splits the dataset into training (70%) and testing (30%) sets. Several models were trained and tested.

Support Vector Classifier (SVC): 100% Accuracy (Selected Model) 

Random Forest: 100% Accuracy 

Gradient Boosting: 100% Accuracy 

K-Nearest Neighbors: 100% Accuracy 

Multinomial Naive Bayes: 100% Accuracy 

The SVC (Linear Kernel) was selected and saved as svc.pkl for the final deployment.

💻 Usage
Run the Notebook/Script: Load the trained svc.pkl model and the CSV databases.

Input Symptoms: When prompted, enter your symptoms separated by commas.

Example Input: itching, skin_rash, nodal_skin_eruptions.

View Results: The system will output the predicted disease followed by the detailed recommendation plan.

Example Output
Plaintext

=================predicted disease============
Fungal infection
=================description==================
Fungal infection is a common skin condition caused by fungi.
=================precautions==================
1 :  bath twice
2 :  use detol or neem in bathing water
...
=================medications==================
5 :  ['Antifungal Cream', 'Fluconazole', 'Terbinafine', 'Clotrimazole', 'Ketoconazole']
...
**

⚠️ Disclaimer
This system is developed for educational and informational purposes only. The predictions and recommendations provided by this AI model should not replace professional medical advice, diagnosis, or treatment. Always consult with a qualified healthcare provider for any medical concerns.
