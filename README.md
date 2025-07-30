WorthSync: AI-Powered Salary Prediction with Explainable NLP

Overview:
WorthSync is a full-stack AI project that predicts salaries based on job profiles. It uses advanced NLP techniques to understand the meaning behind job titles and skills, and a fast, optimized LightGBM model to generate predictions. The system is designed to be interpretable, using SHAP to explain how and why salary predictions are made. The entire solution is deployed as an interactive Streamlit web application.

Key Features:

Predicts salary based on job title, skills, and experience

Uses Sentence-BERT embeddings for contextual understanding

LightGBM model optimized for accuracy and speed

SHAP integration to explain model predictions

User-friendly Streamlit web interface

Project Structure:

worthsync_app.py → Streamlit application script

worthsync_notebook.ipynb → Development and training notebook

model/ → Final trained LightGBM model and SHAP explainer

data/ → Cleaned and preprocessed dataset

assets/ → EDA charts, SHAP visuals, and related images

How to Run the Project (Locally or in Google Colab):

Step 1: Clone the repository
git clone https://github.com/yourusername/worthsync.git
cd worthsync

Step 2: Install required packages
pip install -r requirements.txt

Step 3: Set your ngrok token (needed for Colab Streamlit apps)

Visit: https://dashboard.ngrok.com/get-started/your-authtoken

Copy your ngrok token

In your Colab or terminal, enter:
ngrok config add-authtoken YOUR_NGROK_TOKEN

Step 4: Run the Streamlit app
streamlit run worthsync_app.py

Important: Never share your ngrok token in public code. Use secure methods like environment variables or getpass().

Model Highlights:

LightGBM chosen for its speed and performance

Final Mean Absolute Error: approximately $26,000

NLP embeddings significantly improved prediction accuracy

Real-time SHAP explanations for transparency

Future Enhancements:

Expand prediction beyond tech job roles

Add economic and geographic indicators like cost of living

Host the app permanently on a public cloud

Schedule regular model retraining with updated datasets

Author:

