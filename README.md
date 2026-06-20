# 🧠 Schizophrenia Detection Using EEG Signals

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![ML](https://img.shields.io/badge/Machine%20Learning-Scikit--learn-orange.svg)
![DL](https://img.shields.io/badge/Deep%20Learning-TensorFlow%2FKeras-red.svg)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## 📌 About the Project

Schizophrenia is a serious mental disorder affecting thinking, emotions, and behavior. Early diagnosis is critical for proper treatment and reducing disease severity.

This project uses **EEG (Electroencephalogram) signals** combined with clinical data to automatically classify subjects as **Schizophrenia patients or Healthy individuals** using Machine Learning and Deep Learning techniques.

Traditional diagnosis relies on clinical observation and psychological tests, which are time-consuming and experience-dependent. Our hybrid approach overcomes these limitations by analyzing hidden patterns in brain signals.

---

## 📊 Dataset

- **Source:** BRMH EEG Dataset (publicly available)
- **Subjects:** 945 patients across 7 mental disorder categories
- **Features:** 1,149 columns including:
  - **AB features** — Absolute band power across 6 frequency bands (Delta, Theta, Alpha, Beta, High-beta, Gamma) across 19 brain channels
  - **COH features** — Coherence between electrode pairs across all frequency bands
  - **Clinical data** — Age, sex, education, IQ
- **Disorders covered:** Schizophrenia, Mood disorder, Anxiety disorder, OCD, Addiction disorder, Trauma disorder, Healthy controls
- **Demographics:** 601 Male, 344 Female | Age range: 18–72 years

---

## 🛠️ Tech Stack

| Category | Tools |
|----------|-------|
| Language | Python 3.8+ |
| Data Processing | NumPy, Pandas |
| Machine Learning | Scikit-learn |
| Deep Learning | TensorFlow, Keras |
| Visualization | Matplotlib, Seaborn |
| Web Interface | Streamlit |
| Environment | Google Colab |

---

## 🏗️ System Architecture

```
Input Data (EEG Signals + Clinical Features)
        ↓
Preprocessing (Noise removal, Filtering)
        ↓
Feature Extraction (Statistical features: Mean, Std, Variance)
        ↓
Feature Combination (EEG + Clinical Data)
        ↓
Model Training (RF / SVM / LR / CNN)
        ↓
Prediction & Evaluation
        ↓
Web Interface (Streamlit)
```

---

## 🤖 Models Implemented

| Model | Accuracy |
|-------|----------|
| ✅ **Random Forest** | **93%** |
| 🧠 CNN (Deep Learning) | 86.2% |
| 🔷 Support Vector Machine | 84% |
| 📈 Logistic Regression | 79% |

> **Random Forest achieved the highest accuracy** due to its ability to handle complex, high-dimensional data and reduce overfitting using ensemble of decision trees.

---

## 📈 Evaluation Metrics

- ✅ Accuracy Score
- ✅ Confusion Matrix
- ✅ ROC Curve (AUC)
- ✅ Cross-validation

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/jnanendramanikantaboddu-create/-schizophrenia-eeg-detection.git
cd -schizophrenia-eeg-detection
```

### 2. Install Dependencies
```bash
pip install -r requirements.txt
```

### 3. Run the Notebook
Open `schizophrenia_eeg_detection.ipynb` in Google Colab or Jupyter Notebook.

### 4. Launch the Web App
```bash
streamlit run app.py
```

---

## 📁 Project Structure

```
schizophrenia-eeg-detection/
│
├── schizophrenia_eeg_detection.ipynb   ← Main Colab notebook
├── EEG_machinelearing_data_BRMH.csv    ← Dataset
├── app.py                              ← Streamlit web app
├── requirements.txt                    ← Python dependencies
├── README.md                           ← Project documentation
└── LICENSE
```

---

## 💡 Key Features

- 🔬 **Hybrid Approach** — Combines EEG features with clinical data (age, gender)
- 🤖 **Multiple Models** — Compares ML and DL models for best performance
- 📊 **Rich Feature Set** — 1000+ EEG band power and coherence features
- 🌐 **Web Interface** — User-friendly Streamlit app for predictions
- ✅ **Cross-Validation** — Reliable model evaluation on different data subsets

---

## 🔮 Future Improvements

- Use larger and more diverse EEG datasets
- Explore advanced deep learning architectures (LSTM, Transformers)
- Implement real-time EEG signal processing
- Enhance the UI with better visualization tools
- Deploy as a cloud-based healthcare application

---

## 👨‍💻 Author

**Jnanendra Manikanta Boddu**  
🎓 Aspiring Data Scientist | ML & Healthcare AI Enthusiast  
📍 Bengaluru, India  
🔗 [GitHub](https://github.com/jnanendramanikantaboddu-create)

---

## 📄 License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgements

- BRMH EEG Dataset contributors
- Research papers on EEG-based mental disorder detection
- Open-source ML/DL community
