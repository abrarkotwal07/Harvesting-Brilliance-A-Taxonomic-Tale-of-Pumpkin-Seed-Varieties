# Pumpkin Category Classifier

Badge,Markdown Code
Status,![Status](https://img.shields.io/badge/Status-Operational-success?style=flat-square)
Python,![Python](https://img.shields.io/badge/Python-3.9%2B-blue?style=flat-square&logo=python)
Flask,![Framework](https://img.shields.io/badge/Framework-Flask-black?style=flat-square&logo=flask)
ML Model,![ML](https://img.shields.io/badge/Model-Random%20Forest-orange?style=flat-square)
Dataset,![Data](https://img.shields.io/badge/Source-Excel-green?style=flat-square&logo=microsoftexcel)

**Harvesting Brilliance** is a specialized Machine Learning solution developed to automate the botanical classification of pumpkin seeds. By analyzing complex morphological traits—such as **Eccentricity**, **Solidity**, and **Extent**—this system distinguishes between high-value cultivars like *Çerçevelik* and *Ürgüp Sivrisi* with professional-grade accuracy.

This project bridges the gap between traditional agriculture and data science, providing a digital tool for farmers, researchers, and food scientists to verify seed taxonomy instantly.

---

## ✨ Key Features

* **🧪 Multi-Model Intelligence:** Evaluates 6+ algorithms (Random Forest, SVM, Gradient Boosting) to ensure the most robust classification.
* **📊 Deep Morphological EDA:** Includes a comprehensive analysis of seed geometry, identifying key indicators like "Aspect Ratio" and "Roundness."
* **🌐 Web-Based Deployment:** A streamlined **Flask** application that allows users to input seed measurements and receive instant results.
* **🛡️ Robust Preprocessing:** Automated data cleaning that handles Excel formatting, renames inconsistent columns, and applies **MinMaxScaler** for feature normalization.
* **📉 Precision Evaluation:** Utilizes Confusion Matrices and Classification Reports to validate model reliability.

---

## 🛠️ Tech Stack

* **Core Logic:** Python 3.x
* **Data Science:** Pandas, NumPy, Scikit-learn
* **Visualization:** Matplotlib, Seaborn (Correlation Heatmaps & Pairplots)
* **Backend:** Flask Web Framework
* **Data Source:** Microsoft Excel (`.xlsx`)

---

## 📂 Project Structure

Maintain this structure in your `Harvesting-Brilliance-A-Taxonomic-Tale-of-Pumpkin-Seed-Varieties` directory for optimal performance:

```text
Harvesting-Brilliance-A-Taxonomic-Tale-of-Pumpkin-Seed-Varieties/
│
├── static/
│   └── css/
│       └── style.css          # Custom styling for Glassmorphism & Animations
│
├── templates/
│   ├── index.html             # Main Dashboard & Input Interface
│   └── predict.html           # Result Display Card
│
├── app.py                     # Main Flask Application Server
├── model_building.ipynb       # Jupyter Notebook for Training & Analysis
├── model.pkl                  # Trained Random Forest Model (Auto-generated)
├── scaler.pkl                 # Feature Scaler (Auto-generated)
├── Pumpkin_Seeds_Dataset.xlsx # Raw Dataset Source
└── README.md                  # Project Documentation

```

---

## ⚙️ Installation & Setup

### 1. Environment Setup

Clone the repository:

```bash
git clone https://github.com/abrarkotwal07/Harvesting-Brilliance-A-Taxonomic-Tale-of-Pumpkin-Seed-Varieties.git

```

### 2. Generate the Intelligence

Run the training script to process the **Excel** dataset and save the model:

```bash
python model_building.ipynb

```

*This will perform EDA, clean the data, and export the `model.pkl` and `scaler.pkl` file.*

### 3. Launch the Application

Start the Flask web server:

```bash
python app.py

```

### 4. Interactive Analysis

Open your browser and visit: `http://127.0.0.1:5000/`

---

## 🧠 The Inference Pipeline

1. **Data Acquisition:** Reads raw morphological data from `Pumpkin_Seeds_Dataset.xlsx`.
2. **Feature Engineering:** Fixes column naming errors (e.g., *Aspect_Ration*) and encodes Turkish labels into machine-readable formats.
3. **Normalization:** Scales inputs between 0 and 1 to ensure larger values (like Area) don't overpower smaller values (like Compactness).
4. **Classification:** The Random Forest model processes the features to determine the variety.
5. **User Output:** Displays the final seed type with a clean, professional user interface.

---

## 🔮 Future Scope

* **📸 Computer Vision Integration:** Transitioning from manual numerical input to image-based classification using Convolutional Neural Networks (CNNs).
* **📱 Mobile App Development:** Creating a Flutter or React Native mobile application for on-field usage by farmers without laptop access.
* **🌾 Expanded Taxonomy:** Increasing the dataset to include a wider variety of seeds beyond pumpkin seeds, such as sunflower or watermelon seeds.
* **🏭 Industrial IoT:** Integrating the API with automated sorting machinery in food processing plants for real-time quality control.

---

## 👨‍💻 Author

**Abrar Kotwal**
*Machine Learning Intern*

---

## 📜 Academic Purpose

This project was developed as part of a **Machine Learning Internship Program** for academic evaluation and research into agricultural technology.