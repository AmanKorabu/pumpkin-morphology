🎃 MorphoSeed AI – Intelligent Morphological Classification System

📌 Overview

SeedGenomics is an intelligent, web-based classification system designed to distinguish between pumpkin seed varieties (Çerçevelik and Ürgüp Sivrisi) with high precision.

Moving beyond traditional manual inspection, this project leverages machine learning to analyze quantitative morphological features — such as Area, Perimeter, Major Axis Length, and Aspect Ratio — processing them through a custom inference pipeline to provide instant classification.

🚀 Features

⚡ Real-Time Inference: Optimized Flask backend delivers predictions instantly.

🧠 Advanced AI Model: Powered by a Random Forest Classifier achieving 98.8% accuracy.

🎨 Modern UI/UX: Premium Glassmorphism split-screen dashboard layout.

📊 Smart Feature Scaling: Selective preprocessing using saved scaler.pkl.

📱 Responsive Design: Fully functional across desktop and mobile devices.

🔁 Clean Result Dashboard: Dedicated result screen with classification output.

🛠️ Tech Stack

Frontend

HTML5

CSS3 (Custom Glassmorphism Styling)

Backend

Python 3.x

Flask

Machine Learning

Scikit-learn

NumPy

Pandas

Model Training

Jupyter Notebook (model_building.ipynb)

📂 Project Structure
pumpkin-seed/
│
├── static/
│   └── css/
│       └── style.css
│
├── templates/
│   ├── index.html
│   └── predict.html
│
├── app.py
├── model_building.ipynb
├── model.pkl
├── scaler.pkl
├── Pumpkin_Seeds_Dataset.xlsx
└── README.md
⚙️ Installation & Setup
1️⃣ Prerequisites

Ensure Python 3.9+ is installed.

Install required libraries:

pip install flask scikit-learn pandas numpy openpyxl
2️⃣ Train the Model

Before running the application:

Open model_building.ipynb

Run all cells

Confirm that:

model.pkl

scaler.pkl

are generated in the root folder.

3️⃣ Run the Application
python app.py
4️⃣ Access the Interface

Open your browser and visit:

http://127.0.0.1:5000/

(Note: Flask runs on port 5000 by default, not 5500.)

🧠 How It Works
Step 1 — Data Input

The user enters geometric parameters into the web form.

Step 2 — Preprocessing

The backend:

Extracts the required 8 features used by the model.

Scales Area, Perimeter, and Major_Axis_Length using scaler.pkl.

Step 3 — Inference

The processed features are passed to the trained Random Forest model (model.pkl).

Prediction mapping:

0 → Çerçevelik

1 → Ürgüp Sivrisi

Step 4 — Result Rendering

The predicted class is displayed on a clean, dedicated result page.

🔮 Future Scope

📷 Image-based classification using Convolutional Neural Networks (CNN)

📊 Display prediction probability / confidence score

☁️ Deploy to cloud (Render / Railway / AWS)

📈 Add model performance dashboard

🔁 Automated retraining pipeline

📝 License

This project is developed for educational and academic submission purposes.

👨‍💻 Developed By

Aman Mehboob Korabu
Aspiring Full Stack & Machine Learning Developer