# 🚗 Smart Parking Detection using Image Classification | Python & Scikit-learn

![Python](https://img.shields.io/badge/Python-3.10%2B-blue?logo=python&logoColor=white)
![Scikit-learn](https://img.shields.io/badge/Scikit--learn-1.1.3-F7931E?logo=scikit-learn&logoColor=white)
![Scikit-image](https://img.shields.io/badge/Scikit--image-0.19.3-0096D6?logo=scikit-image&logoColor=white)
![Numpy](https://img.shields.io/badge/NumPy-1.23.4-013243?logo=numpy&logoColor=white)
![Status](https://img.shields.io/badge/Project_Status-Active-brightgreen)
![License](https://img.shields.io/badge/License-MIT-yellow)

An **end-to-end computer vision project** that classifies parking spaces as **“Empty” or “Not Empty”** using **Scikit-learn (SVM)** and **Scikit-image**.  
This model automates parking detection, supporting **smart city infrastructure** and real-time parking space management.

---

## 🚀 Project Overview

The **Smart Parking Detection System** is built using **Python**, **Scikit-learn**, and **Scikit-image** to detect whether a parking space is vacant or occupied.  
It leverages **Support Vector Machine (SVM)** for classification and **GridSearchCV** for hyperparameter tuning, achieving optimized model performance.

---

## 🧠 Key Features

- 🅿️ **Automatic Parking Space Detection:** Classifies images as *empty* or *not empty* using a trained SVM classifier.  
- ⚙️ **Machine Learning Pipeline:** Implements data preprocessing, model training, tuning, and evaluation in one workflow.  
- 🔍 **Hyperparameter Optimization:** Uses **GridSearchCV** to find the best `C` and `gamma` parameters for the SVM model.  
- 💾 **Model Persistence:** Saves the best-performing model as `model.p` using Python’s `pickle` for future deployment.  
- 📈 **Performance Evaluation:** Calculates test accuracy using **accuracy_score** to assess real-world reliability.  

---

## 🏗️ Tech Stack

| Category | Tools / Libraries |
|-----------|------------------|
| **Programming Language** | Python |
| **Libraries** | Scikit-learn, Scikit-image, NumPy, Pickle |
| **Algorithm** | Support Vector Machine (SVM) |
| **Model Selection** | GridSearchCV |
| **Image Processing** | Resize, Flattening |
| **Evaluation Metrics** | Accuracy Score |

---

## 🧩 Architecture & Workflow

```plaintext
Raw Parking Images
        ↓
Image Preprocessing (Resize, Flatten)
        ↓
Train-Test Split (80/20)
        ↓
SVM Classifier + GridSearchCV
        ↓
Best Model Selection
        ↓
Model Evaluation (Accuracy)
        ↓
Model Saved (model.p)
```

## ⚙️ Installation & Setup
1️⃣ Clone the Repository
bash
Copy code
git clone https://github.com/mrharit/Image-classification-with-Python-and-Scikit-learn

2️⃣ Create Virtual Environment
bash
Copy code
python -m venv venv
source venv/bin/activate    # Mac/Linux
venv\Scripts\activate       # Windows

3️⃣ Install Dependencies
bash
Copy code
pip install -r requirements.txt
4️⃣ Update Dataset Path
In the script, update the dataset directory path:

python
Copy code
input_dir = 'path_to_your_dataset/clf-data'

5️⃣ Run the Training Script
bash
Copy code
python app.py
📦 Requirements
Your requirements.txt file should include:

ini
Copy code
scikit-learn==1.1.3
scikit-image==0.19.3
numpy==1.23.4
💡 How It Works
Data Preparation: Reads images from the empty and not_empty folders and preprocesses them (resize → flatten).

Training: Splits data (80/20) into training and test sets using train_test_split.

Model Optimization: Runs GridSearchCV to test multiple hyperparameter combinations (C and gamma).

Evaluation: Evaluates accuracy using accuracy_score.

Persistence: Saves the trained model as model.p using pickle for future use in a parking detection system.

📊 Example Output
Terminal Output Example:

matlab
Copy code
95.6% of samples were correctly classified
Model Saved As:

bash
Copy code
./model.p
🌍 Real-World Application
This project addresses a real-world problem in smart parking systems by automating vehicle detection.
It can be integrated with:

🏙️ Smart City Traffic Systems

🚘 IoT-enabled Parking Lots

🧠 AI Dashboards for Space Utilization

🧠 Learning & Takeaways
Through this project, I gained practical experience in:

Machine Learning with Scikit-learn (SVM, GridSearchCV)

Image Processing with Scikit-image

Data Pipeline Design and Model Deployment

Real-world AI problem-solving for Smart Cities

📈 Future Enhancements
🔍 Integrate OpenCV for live video frame detection.

☁️ Deploy the model on AWS / Azure for real-time parking management.

📊 Build a Power BI / Streamlit dashboard for visualization.

🧠 Extend the model for multi-class vehicle detection (car, bike, truck).

