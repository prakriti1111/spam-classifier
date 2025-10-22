# Email/SMS Spam Classifier

This is a web application built using **Streamlit** that allows users to classify messages as **Spam** or **Not Spam**. It uses a **machine learning model** trained on a labeled dataset of SMS/Email messages and performs text preprocessing including tokenization, stopword removal, and stemming.

---
## Deployed Link
https://prakriti1111-spam-classifier.streamlit.app/

---
## Features

- Classify input messages as **Spam** or **Not Spam**.
- Preprocessing pipeline includes:
  - Lowercasing
  - Tokenization
  - Removal of non-alphanumeric characters
  - Stopwords removal
  - Stemming using **Porter Stemmer**
- Uses a **TF-IDF vectorizer** for feature extraction.
- Real-time predictions with **Streamlit UI**.

---

## Screenshots



---

## Installation

### Prerequisites

- Python 3.8+
- pip

### Clone the Repository

```bash
git clone https://github.com/prakriti1111/spam-classifier
cd spam classifier
```
Install Dependencies
Create a requirements.txt file with the following content:
```bash
streamlit
nltk
scikit-learn
numpy
pandas
```
Then install dependencies:

```bash
pip install -r requirements.txt
```
NLTK Downloads
Some NLTK resources are required. Open a Python shell and run:
```bash
import nltk
nltk.download('punkt')
nltk.download('stopwords')
```
Usage
Run the Streamlit app:
```bash
streamlit run app.py
```
This will launch the app in your browser. Enter any message in the text area and click Predict to see if it is Spam or Not Spam.

### Project Structure
spam-classifier/<br>
│<br>
├── app.py                # Main Streamlit application<br>
├── model.pkl             # Trained machine learning model<br>
├── vectorizer.pkl        # TF-IDF vectorizer<br>
├── requirements.txt      # Project dependencies<br>
└── README.md             # Documentation<br>
How it Works
User inputs a message in the text area.

The app preprocesses the text:

Converts to lowercase

Tokenizes the text

Removes stopwords and punctuation

Applies stemming

Preprocessed text is transformed using the saved TF-IDF vectorizer.

The machine learning model predicts whether the message is spam.

The result is displayed in the app.

## Author
### Prakriti Gupta
