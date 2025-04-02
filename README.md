# MediSense: Symptom-Based Disease Prediction Tool

## Overview
MediSense is an AI-powered medical symptom checker that helps users identify potential diseases based on their symptoms. Built with Flask and machine learning, the application provides not only disease predictions but also comprehensive information about the condition, including descriptions, precautions, medications, recommended workouts, and dietary advice.

## Features
- Simple symptom input interface
- ML-based disease prediction (supports 130+ symptoms and 40+ diseases)
- Detailed disease information including:
  - Medical descriptions
  - Recommended precautions
  - Medication suggestions
  - Exercise recommendations
  - Dietary guidelines

## Technology Stack
- **Backend**: Python, Flask
- **Frontend**: HTML, Bootstrap 5
- **Machine Learning**: Support Vector Classification (SVC)
- **Data**: CSV datasets for symptoms, diseases, precautions, medications, etc.

## Installation and Setup

### Prerequisites
- Python 3.6+
- pip package manager

### Installation Steps
1. Clone the repository
   ```
   git clone https://github.com/yasithS/medisense.git
   cd medisense
   ```

2. Create and activate a virtual environment (optional but recommended)
   ```
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install the required dependencies
   ```
   pip install -r requirements.txt
   ```

4. Run the application
   ```
   python main.py
   ```

5. Access the application through your web browser
   ```
   http://localhost:3000
   ```

## Usage
1. Enter your symptoms in the input field, separated by commas (e.g., "itching, skin_rash, fatigue")
2. Click the "Submit" button
3. View the predicted disease and explore the detailed information in the accordion sections

## Project Structure
```
medisense/
├── data/                      # CSV datasets
│   ├── description.csv        # Disease descriptions
│   ├── diets.csv              # Dietary recommendations
│   ├── medications.csv        # Medication information
│   ├── precautions_df.csv     # Precautionary measures
│   ├── symtoms_df.csv         # Symptom descriptions
│   └── workout_df.csv         # Exercise recommendations
├── model/                     # Machine learning models
│   └── svc.pkl                # Trained SVC model
├── static/                    # Static files (CSS, images)
│   └── logoFinal.png          # MediSense logo
├── templates/                 # HTML templates
│   └── index.html             # Main application interface
├── .gitattributes             # Git attributes file
├── .gitignore                 # Git ignore file
├── LICENSE                    # Apache 2.0 license
├── README.md                  # Project documentation
└── main.py                    # Main application file
```

## Supported Symptoms
The application supports a wide range of symptoms including:
- Itching, skin rash, nodal skin eruptions
- Continuous sneezing, shivering, chills
- Joint pain, stomach pain, acidity
- And many more

## License
This project is licensed under the Apache License 2.0 - see the LICENSE file for details.

## Disclaimer
MediSense is designed for educational and informational purposes only. It is not a substitute for professional medical advice, diagnosis, or treatment. Always seek the advice of your physician or other qualified health provider with any questions you may have regarding a medical condition.
