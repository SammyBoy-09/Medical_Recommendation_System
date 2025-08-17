# Medical Recommendation System

A Flask-based web application that provides medical recommendations including disease prediction, medications, diet suggestions, and workout plans based on user symptoms.

## Features

- **Disease Prediction**: Uses machine learning (SVC model) to predict diseases based on symptoms
- **Medical Recommendations**: Provides comprehensive recommendations including:
  - Disease descriptions
  - Precautions to take
  - Medication suggestions
  - Diet recommendations
  - Workout plans

## Technology Stack

- **Backend**: Python, Flask
- **Machine Learning**: Scikit-learn (Support Vector Classifier)
- **Data Processing**: Pandas, NumPy
- **Frontend**: HTML, CSS, JavaScript, jQuery, Bootstrap
- **Model Storage**: Pickle

## Installation

1. Clone the repository:
```bash
git clone <repository-url>
cd Medical-Recommendation
```

2. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

3. Install dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Run the Flask application:
```bash
python main.py
```

2. Open your web browser and navigate to `http://localhost:5000`

3. Select your symptoms from the available options

4. Get comprehensive medical recommendations

## Project Structure

```
├── main.py                 # Main Flask application
├── requirements.txt        # Python dependencies
├── datasets/              # CSV files with medical data
│   ├── description.csv
│   ├── diets.csv
│   ├── medications.csv
│   ├── precautions_df.csv
│   ├── Symptom-severity.csv
│   ├── symtoms_df.csv
│   ├── Training.csv
│   └── workout_df.csv
├── models/                # Trained ML models
│   └── svc.pkl
├── static/                # Static files (CSS, JS, images)
├── templates/             # HTML templates
└── .gitignore
```

## Dataset Information

The application uses several medical datasets:
- **Symptoms Data**: Comprehensive list of medical symptoms
- **Disease Descriptions**: Detailed information about various diseases
- **Medications**: Medicine recommendations for different conditions
- **Diet Plans**: Nutritional recommendations
- **Workout Plans**: Exercise suggestions for different health conditions
- **Precautions**: Safety measures and preventive care

## Model Information

The application uses a Support Vector Classifier (SVC) model trained on medical symptom data to predict diseases. The model is pre-trained and stored as a pickle file.

## Important Note

⚠️ **Disclaimer**: This application is for educational and informational purposes only. It should not be used as a substitute for professional medical advice, diagnosis, or treatment. Always consult with qualified healthcare professionals for medical concerns.

## Contributing

1. Fork the repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

## License

This project is licensed under the MIT License - see the LICENSE file for details.
