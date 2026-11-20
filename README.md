# 🩸 BloodAI – AI-Powered Blood Report Analyzer

### Turning Complex Blood Reports into Simple Health Insights

BloodAI is an AI-powered blood report analyzer that helps users understand their laboratory reports through Machine Learning and Artificial Intelligence.

The application extracts important blood parameters, compares values against configured reference ranges, identifies potentially abnormal values, and generates easy-to-understand explanations.

Built using Python, Streamlit, Random Forest and LLM-based explanations, BloodAI aims to make blood report interpretation more accessible.

> **Disclaimer:** BloodAI is an educational AI-assisted tool, not a medical diagnostic system. It does not replace professional medical advice.

---

## 🚀 Key Features

- 🔐 **Email OTP Authentication** – Secure login using email verification.
- 📄 **PDF Report Upload** – Upload blood reports for automated text extraction.
- ✍️ **Raw Text Input** – Paste blood report text directly.
- 🧪 **Blood Parameter Extraction** – Extract important laboratory parameters.
- 📊 **Reference Range Comparison** – Identify values marked Low, Normal or High.
- 🤖 **Random Forest Classification** – Analyze extracted blood parameter patterns.
- 🧠 **AI-Powered Explanations** – Generate understandable explanations using an LLM.
- 🌙 **Dark & Light Mode** – Switch between different interface themes.
- 📈 **Interactive Dashboard** – View extracted parameters and analysis results.

---

## 🧬 Blood Parameters

The prototype supports the following parameters:

| Parameter | Description |
|---|---|
| Hemoglobin | Hemoglobin level |
| RBC | Red Blood Cell count |
| WBC | White Blood Cell count |
| Platelets | Platelet count |
| Glucose | Blood glucose level |
| Cholesterol | Total cholesterol |

Additional parameters can be incorporated in future versions.

---

## ⚙️ System Architecture

```text
                 USER
                   |
                   v
           Email OTP Login
                   |
                   v
             Dashboard
                   |
          +--------+--------+
          |                 |
          v                 v
       Upload PDF       Paste Text
          |                 |
          v                 |
      PDF Extraction         |
          |                 |
          +--------+--------+
                   |
                   v
          Parameter Extraction
                   |
                   v
           Data Processing
                   |
                   v
        Reference Range Checking
                   |
                   v
          Random Forest Model
                   |
                   v
           ML Classification
                   |
                   v
             Groq LLM
                   |
                   v
          AI-Based Explanation
                   |
                   v
             Final Results
```

---

## 🤖 Machine Learning

BloodAI uses a Random Forest Classifier to analyze extracted blood parameters.

### ML Workflow

1. Collect and prepare the training dataset.
2. Perform data preprocessing.
3. Select relevant blood parameters.
4. Split the dataset into training and testing sets.
5. Train the Random Forest Classifier.
6. Generate predictions.
7. Evaluate model performance.

### Model Evaluation

The model should be evaluated using:

- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

**Note:** Model performance depends on the training dataset. Experimental results from synthetic data should not be interpreted as clinical accuracy.

---

## 🛠️ Technology Stack

| Category | Technologies |
|---|---|
| Programming Language | Python |
| Frontend | Streamlit |
| Machine Learning | Scikit-learn |
| ML Algorithm | Random Forest |
| Data Processing | Pandas, NumPy |
| PDF Processing | PyPDF |
| AI Integration | Groq API |
| Model Storage | Joblib |
| Authentication | Email OTP |
| Version Control | Git, GitHub |
| Deployment Target | Render |

---

## 📂 Project Structure

```text
BloodAI/
│
├── AI_Blood_Sample_Analyzer_Advanced/
│   │
│   ├── app.py
│   ├── .env.example
│   ├── .gitignore
│   ├── requirements.txt
│   ├── sample_report.txt
│   └── README.md
│
└── README.md
```

---

## 💻 Installation & Setup

### 1. Clone the Repository

```bash
git clone https://github.com/shreyasahani26/BloodAI.git
```

### 2. Navigate to the Project Folder

```bash
cd BloodAI/AI_Blood_Sample_Analyzer_Advanced
```

### 3. Create a Virtual Environment

```bash
python -m venv .venv
```

Activate it on Windows:

```powershell
.venv\Scripts\activate
```

### 4. Install Dependencies

```bash
pip install -r requirements.txt
```

### 5. Configure Environment Variables

Create a `.env` file using `.env.example` as a reference.

Add your required credentials:

```env
SMTP_EMAIL=your_email@gmail.com
SMTP_APP_PASSWORD=your_gmail_app_password
GROQ_API_KEY=your_groq_api_key
```

Never upload your actual `.env` file or API keys to GitHub.

### 6. Run the Application

```bash
python -m streamlit run app.py
```

Open your browser:

```text
http://localhost:8501
```

---

## 🔑 Environment Configuration

The application may require:

- Gmail App Password for sending OTP emails.
- Groq API key for LLM-based explanations.

Keep all credentials private and configure them through environment variables or your deployment platform's secret management.

---

## 🔮 Future Improvements

- Support for additional blood parameters.
- OCR for scanned PDF reports and images.
- Downloadable PDF analysis reports.
- Historical report tracking.
- Improved data extraction accuracy.
- Interactive charts and visualizations.
- Enhanced model evaluation using validated datasets.
- More comprehensive AI explanations.

---

## 👨‍💻 Project Contributors

**Tanish Kumar**  
B.Tech – Computer Science Engineering (AIML)

**Shreya Sahani**

---

## 📌 Project Information

**Project Name:** BloodAI  
**Domain:** Artificial Intelligence & Healthcare  
**Category:** Machine Learning / AI Application  
**Framework:** Streamlit  
**Repository:** https://github.com/shreyasahani26/BloodAI

---

## ⚠️ Medical Disclaimer

BloodAI is developed for educational and experimental purposes.

The system does not diagnose diseases, prescribe medication, or replace a qualified healthcare professional.

Reference ranges may vary depending on laboratory standards and individual circumstances. Users should consult healthcare professionals for medical interpretation.

---

⭐ If you find this project interesting, consider giving the repository a star!

