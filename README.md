# Mental Health App

A Streamlit-based mental health journal analyzer that predicts likely mental health-related tags from a text entry using a trained machine learning model.

## Overview

This project loads a trained classifier, TF-IDF vectorizer, and multi-label binarizer to analyze journal text and identify relevant mental health conditions such as anxiety, depression, stress, and other supported labels.

The app is implemented in `mental_health_app.py` and is designed for quick local use in a browser.

## Features

- Text input for mental health journal entries
- Multi-label prediction using a trained classifier
- Streamlit UI for easy interaction
- Model artifacts included in the repository

## Project Files

- `mental_health_app.py` — Streamlit app entry point
- `classifier_model.pkl` — trained model
- `tfidf_vectorizer.pkl` — text vectorizer
- `multilabel_binarizer.pkl` — label mapping
- `requirements.txt` — Python dependencies

## Requirements

Python 3.9+ is recommended.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/SehajjotSingh/mental-health-app.git
   cd mental-health-app
   ```

2. Create and activate a virtual environment (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate   # On macOS/Linux
   # venv\Scripts\activate   # On Windows
   ```

3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```

## Run the App

```bash
streamlit run mental_health_app.py
```

Then open the local URL shown in the terminal (typically `http://localhost:8501`).

## Example Usage

Enter a journal entry such as:

> I feel overwhelmed and anxious all day. I have trouble sleeping and feel exhausted.

Click "Analyze" to receive predicted mental health tags.

## Notes

- This app is intended for research or educational use and should not replace professional mental health assessment.
- The model's predictions depend on the quality and scope of the training data used to build it.
