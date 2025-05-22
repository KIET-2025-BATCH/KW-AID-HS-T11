# KW-AID-HS-T11

===============================
Covid-19 Chest X-ray Detection
===============================

This project is a web application that allows users to upload chest X-ray images and get AI-based predictions (COVID, Normal, Lung Opacity, or Viral Pneumonia). It includes user authentication, image upload, prediction using a trained deep learning model, and storing reports in Firebase.

------------
How to Run:
------------

1. UNZIP the project folder.

2. Install dependencies:
   - Open a terminal in the project directory
   - Run: pip install -r requirements.txt

3. Firebase Setup:
   - Place your Firebase credentials JSON file as 'firebase_credentials.json' in the root directory.
   - Ensure your Firebase Firestore and Storage are correctly configured.

4. Run the model.ipynb file   

5. Start the Flask server:
   - Run: python app.py

6. Open `home.html` in your browser OR connect to http://127.0.0.1:5000/ if you integrate it with Flask routing.

-----------------------
Main Functionalities:
-----------------------

- User login and session handling
- X-ray image upload and AI prediction
- Result confidence shown
- Report history (stored in Firebase)
- Performance tracking of model accuracy

-------------------
Project Structure:
-------------------

project/
│
├── COVID-19_Radiography_Dataset
├── dataset_prepared
├── model.ipynb
│
├── backend
│   └── app.py
│   └── covid-detection-through-x-rays-firebase-adminsdk-fbsvc-53327b258a.json
│   └── firebase_key.json
│   └── covid19_cnn_model.h5
│   └── requirements.txt
│
├── frontend
│   └── static/
│       └── images/
│           └── cartoon-image.jpg
│           └── Causes.jpeg
│           └── covid-19.jpeg
│           └── logo.jpg
│           └── precautions.jpg
│           └── scope.jpeg
│   └── home.css
│   └── pastreports.css
│   └── report.css
│   └── styles.css
│   └── upload.css
│   └── uploades_xrays/
│   └── home.html
│   └── login.html
│   └── pastreports.html
│   └── register.html
│   └── report.html
│   └── upload.html
│   └── auth.js
│   └── firebase-config.js
│   └── logout.js
│   └── pastreports.js
│   └── report.js
│   └── upload.js
│   └── uploaded_xrays
└── README.md            

----------------
Notes:
----------------

- Ensure TensorFlow works with your system (use CPU/GPU version accordingly).
- Confirm Firebase project setup before using login/report features.


