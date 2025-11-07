HR Attrition Streamlit App
==========================

Files contained in this ZIP (no folders):
- app.py        : Main Streamlit application (single-file).
- README.md     : This file.
- requirements.txt : List of required packages (no versions).

How to deploy:
1. Create a new GitHub repository and upload these files to the repo root.
2. Go to https://streamlit.io/cloud and connect your GitHub repo. Choose the repo and branch, and set the main file to `app.py`.
3. Streamlit Cloud will install packages from requirements.txt and launch the app.

Notes:
- The app will drop rows with nulls before training/prediction (per your request to ignore nulls).
- The app is flexible: you will be asked to map job-role, satisfaction and target columns if they cannot be auto-detected.
- The 'Models' tab trains LogisticRegression, RandomForest, and GradientBoosting (sklearn).
- For production, consider persisting trained models to disk and using the same encoders at prediction time.
