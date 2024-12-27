# Personalized Medical Recommendation System

This is a Flask-based web application that predicts diseases based on user-provided symptoms using a machine learning model. The system integrates various datasets to provide detailed information about diseases, including descriptions, precautions, medications, diet recommendations, and workout suggestions.

## Features

- **Disease Prediction**: Predicts diseases based on symptoms using a Support Vector Classifier (SVC) model.
- **Detailed Information**:
  - Disease description
  - Precautions to take
  - Medications
  - Recommended diet
  - Suggested workouts
- **Static Pages**:
  - About
  - Contact
  - Developer information
  - Blog
- **Error Handling**: Validates input symptoms and provides user-friendly error messages for invalid or missing inputs.

## Prerequisites

- Python 3.8 or later
- Flask
- Pandas
- Scikit-learn
- Joblib

## Installation

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/praveen-ku12345/AI-Driven-Health-Care-Assistant.git
   cd disease-prediction-system
   ```

2. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Place Model and Data Files**:
   - Ensure the `svc.pkl` file is placed in the project directory.
   - Place the following CSV files in the `data` folder:
     - `symptoms_df.csv`
     - `precautions_df.csv`
     - `workout_df.csv`
     - `description.csv`
     - `medications.csv`
     - `diets.csv`

4. **Run the Application**:
   ```bash
   python app.py
   ```

5. **Access the Application**:
   Open a web browser and navigate to `http://127.0.0.1:5000`.

## Usage

1. Enter symptoms in the provided input field as a comma-separated list (e.g., "fever, cough, headache").
2. Click on the "Predict" button to get the disease prediction and detailed information.
3. Navigate through the static pages for additional information about the app and its developers.

## Project Structure

```
.
├── app.py                 # Main Flask application
├── svc.pkl                # Pre-trained SVC model
├── data/                  # Folder containing CSV files
│   ├── symptoms_df.csv
│   ├── precautions_df.csv
│   ├── workout_df.csv
│   ├── description.csv
│   ├── medications.csv
│   └── diets.csv
├── templates/             # HTML templates
│   ├── index.html
│   ├── about.html
│   ├── contact.html
│   ├── developer.html
│   └── blog.html
├── static/                # Static assets (CSS, JS, images)
├── requirements.txt       # List of dependencies
└── README.md              # Project documentation
```

## Example Input and Output

### Input:
```
fever, cough, headache
```

### Output:
- **Predicted Disease**: Influenza
- **Description**: Influenza, commonly known as the flu, is a viral infection.
- **Precautions**:
  - Wash your hands frequently
  - Avoid crowded places
- **Medications**:
  - Antiviral drugs
- **Diet Recommendations**:
  - Stay hydrated
  - Consume light, nutritious meals
- **Workout Suggestions**:
  - Light stretching
  - Restful activities

## Future Enhancements

- Add autocomplete for symptom input.
- Improve the user interface with React or Angular.
- Enhance the prediction model with updated datasets.
- Add support for multiple languages.
- Implement logging for debugging and usage analytics.


## Contributing

Contributions are welcome! Please fork this repository and submit a pull request with your changes.

## Contact

For questions or feedback, please contact Kunusothu Praveen at praveenkunusothu97@gmail.com.
