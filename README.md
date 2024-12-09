
# Email/SMS Spam Classifier

This project is a **Streamlit-based application** for classifying emails and SMS messages as "Spam" or "Not Spam" using machine learning.

## Features
- **Text Preprocessing**: Cleans and transforms user input by tokenizing, removing stopwords, and applying stemming.
- **TF-IDF Vectorization**: Converts text into numerical features for model prediction.
- **Spam Detection**: Predicts whether a given message is spam or not using a pre-trained model.

## Prerequisites
Make sure you have the following installed:
- Python 3.8+
- Streamlit
- NLTK
- scikit-learn
- pickle

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/spam-classifier.git
   cd spam-classifier
   ```
2. Install the required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Download NLTK data:
   ```bash
   python -c "import nltk; nltk.download('punkt'); nltk.download('stopwords')"
   ```

## Usage
1. Place the required files (`model.pkl` and `vectorizer.pkl`) in the same directory as `app.py`.
2. Run the Streamlit app:
   ```bash
   streamlit run app.py
   ```
3. Open the app in your browser using the provided URL (default: `http://localhost:8501`).

## How It Works
1. Enter the message in the text area on the web app.
2. Click the **Predict** button.
3. The app preprocesses the input text, vectorizes it, and uses a machine learning model to classify it.
4. The result is displayed as either **Spam** or **Not Spam**.

## File Descriptions
- `app.py`: The main Streamlit application script.
- `model.pkl`: Pre-trained machine learning model (required for predictions).
- `vectorizer.pkl`: TF-IDF vectorizer (required for text transformation).

## Dependencies
A sample `requirements.txt` file:
```txt
streamlit
nltk
scikit-learn
```

## Screenshots
