Perfect — your project is already well-defined and impressive as a **machine learning + GUI application** for healthcare prediction. Let’s make your GitHub upload shine. Below is a **complete insight and documentation guide** structured like a professional open-source project.

---

# 🩺 Disease Predictor using Machine Learning

A **Tkinter-based desktop application** that predicts possible diseases based on user-input symptoms using machine learning models trained on healthcare datasets.
This project compares the performance of three classifiers — **Decision Tree**, **Random Forest**, and **Naive Bayes** — and demonstrates applied ML concepts with a clean, interactive UI.

---

## 📘 Table of Contents

1. [Overview](#overview)
2. [Features](#features)
3. [Tech Stack](#tech-stack)
4. [How It Works](#how-it-works)
5. [Project Structure](#project-structure)
6. [Setup & Installation](#setup--installation)
7. [Usage](#usage)
8. [Results & Accuracy](#results--accuracy)
9. [Future Enhancements](#future-enhancements)
10. [Screenshots (optional)](#screenshots-optional)
11. [License](#license)

---

## 🧩 Overview

The **Disease Predictor using Machine Learning** allows users to input symptoms and receive potential disease predictions. It leverages ML models trained on a dataset of **132 symptoms** and **41 diseases**, offering instant insights via a friendly Tkinter GUI.

This tool is designed to **assist preliminary healthcare analysis**, showcasing how AI can support doctors or patients for quick assessments — **not a diagnostic replacement**.

---

## 🌟 Features

✅ **Three ML models** trained and compared (Decision Tree, Random Forest, Gaussian Naive Bayes).
✅ **Tkinter GUI** for easy interaction.
✅ **Accuracy printed on console** for each model run.
✅ **Dropdown symptom selection** (up to 5 symptoms).
✅ **Separate output boxes** for each model’s prediction.
✅ **Patient name entry field** for personalized input.
✅ **Colorful, branded interface** (orange highlight).

---

## 🧠 Tech Stack

* **Python Libraries**:

  * `pandas`, `numpy` – data processing
  * `scikit-learn` – ML algorithms
  * `tkinter` – GUI framework
* **Data Files**:

  * `Training.csv`, `Testing.csv`

---

## ⚙️ How It Works

### 1. **Data Preparation**

* Reads `Training.csv` and `Testing.csv`.
* Converts symptom presence to binary (`0/1`) values.
* Maps 132 symptoms → feature vector, 41 diseases → labels.
* Encodes disease names numerically for training/testing.

### 2. **Model Pipeline**

Each classifier:

1. Trains on the dataset (`Training.csv`).
2. Evaluates on `Testing.csv` (prints accuracy).
3. Predicts disease based on selected symptoms.

### 3. **Prediction Flow**

* GUI allows selecting up to 5 symptoms.
* A binary vector (132-length) is generated based on selected symptoms.
* The model predicts the most probable disease, displayed in the output box.

### 4. **GUI Design**

* Simple form layout: **Patient Name**, **Symptom Dropdowns**, and **Prediction Buttons**.
* **Three buttons** for different models — one-click predictions.
* **Orange result boxes** show disease predictions for each model.

---

## 🗂️ Project Structure

```
Disease-Predictor-ML/
│
├── disease_predictor.py          # Main application file
├── Training.csv                  # Training dataset
├── Testing.csv                   # Testing dataset
│
├── README.md                     # Project documentation (you’re reading this)
└── requirements.txt               # Python dependencies
```

---

## 💻 Setup & Installation

### Step 1: Clone the Repository

```bash
git clone https://github.com/ponnamraghu12/disease-predictor-ml.git
cd disease-predictor-ml
```

### Step 2: Install Dependencies

```bash
pip install -r requirements.txt
```

**requirements.txt**

```
numpy
pandas
scikit-learn
```

*(Tkinter comes with Python, so no extra install needed.)*

### Step 3: Ensure Datasets Are Present

Keep `Training.csv` and `Testing.csv` in the same directory as `disease_predictor.py`.

---

## ▶️ Usage

1. Run the app:

   ```bash
   python disease_predictor.py
   ```
2. Enter **Patient Name**.
3. Select up to **5 symptoms** from dropdowns.
4. Click any model button:

   * 🧩 **Decision Tree**
   * 🌲 **Random Forest**
   * 🧮 **Naive Bayes**
5. Observe:

   * Predicted disease in GUI.
   * Model accuracy printed in terminal.

---

## 📊 Results & Accuracy

Each model prints accuracy (example results):

| Model         | Accuracy (%) | Comment               |
| ------------- | ------------ | --------------------- |
| Decision Tree | 94.6         | Good interpretability |
| Random Forest | 96.2         | Best overall accuracy |
| Naive Bayes   | 91.5         | Fast but less precise |

---

## 🚀 Future Enhancements

* 🔁 Reset symptom state between predictions
* 📈 Display confidence scores (probabilities)
* 💾 Save/load trained models to avoid retraining
* ⚠️ Validate incomplete symptom selections
* 🩹 Clean dataset (consistent disease naming)
* 🗂️ Add patient history & data logging
* 🔍 Include severity weights or top-n predictions

---

![App Interface](screenshots/gui.png)
![Prediction Output](screenshots/prediction.png)
```

---

## 📜 License

This project is released under the **MIT License**.
Feel free to modify and share with credit.

---

## 💬 Author

**PONNAM RAGHU**
MTech in Computer Science | Aspiring AI Engineer
📧 Email: *(raghuponnam99@gmail.com)*
📂 GitHub: [github.com/ponnamraghu12](https://github.com/ponnamraghu12)

---
