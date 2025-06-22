Certainly! Here's the updated `README.md` section with the **dataset link** included:

---

### 📚 Dataset

This project uses a dataset from **Kaggle**:

* **Dataset Name**: [NER Annotated CVs](https://www.kaggle.com/datasets/mehyarmlaweh/ner-annotated-cvs)
* **Source**: Kaggle
* **Usage**: Resumes in PDF format are used for training the custom NER model and for testing resume ranking against job descriptions.

All resumes are anonymized and publicly available under the dataset’s terms of use.

---

Now here is the **full updated `README.md`** with the dataset section integrated:

---

```markdown
# Automated Resume Analysis and Matching Using NLP and Custom NER

This project automates the process of resume screening using Natural Language Processing (NLP) and a custom Named Entity Recognition (NER) model built with spaCy. It processes PDF resumes, extracts structured information like Name, Email, Skills, Education, and Experience, and ranks them against a job description using TF-IDF and cosine similarity.

---

## 📌 Features

- ✅ PDF text extraction using **PyMuPDF** and **Tesseract OCR**
- 🧠 Custom **spaCy NER** model for extracting resume entities
- 🔍 Resume ranking using **TF-IDF** and **cosine similarity**
- 📊 Outputs include ranked results, JSON annotations, and model files
- 💡 Designed to run on **Google Colab (Free Tier)** — no GPU needed

---

## 🛠️ Technologies Used

- Python 3.x
- spaCy (custom NER model)
- PyMuPDF (PDF extraction)
- Tesseract OCR (scanned PDFs)
- scikit-learn (TF-IDF, similarity scoring)
- Google Colab (CPU-based runtime)

---

## 📚 Dataset

This project uses a dataset from **Kaggle**:

- **Dataset Name**: [NER Annotated CVs](https://www.kaggle.com/datasets/mehyarmlaweh/ner-annotated-cvs)
- **Source**: Kaggle  
- **Usage**: Resumes in PDF format are used for training the custom NER model and for testing resume ranking against job descriptions.

All resumes are anonymized and publicly available under the dataset’s terms of use.

---

## 📂 Folder Structure

```

project/
│
├── resume\_analysis.py              # Main pipeline script
├── requirements.txt                # Python dependencies
├── README.md                       # This file
│
├── data/
│   ├── sample\_resumes/             # Folder with PDF resumes
│   └── job\_description.txt         # Role/job description for matching
│
├── models/
│   └── ner\_model/                  # Trained spaCy NER model
│
└── outputs/
├── annotations/                # JSON outputs of extracted entities
└── rankings/                   # Ranked resumes with similarity scores

````

---

## 🚀 How to Run

### 1. Clone the Repository
```bash
git clone https://github.com/YOUR_USERNAME/automated-resume-analysis.git
cd automated-resume-analysis
````

### 2. Install Dependencies

```bash
pip install -r requirements.txt
```

### 3. Run the Script

You can either run it locally or on Google Colab (recommended for limited hardware).

```bash
python resume_analysis.py
```

### 4. Outputs

* Annotated entities are saved in JSON format.
* Trained model is stored in `models/ner_model/`.
* Ranked resume scores are printed to the console and saved in `outputs/rankings/`.

---

## 📈 Performance Highlights

* **5,050 resumes** processed in **4 hours 48 minutes** on free Google Colab CPU
* **NER F1-score**: 99.94% (Precision: 99.97%, Recall: 99.91%)
* **Resume Matching Time**: <10 minutes for 5,048 resumes
* **Top Similarity Score**: 0.1895 (TF-IDF + Cosine Similarity)

---

## ✅ Use Cases

* HR departments or startups needing low-cost resume filtering
* Educational or research projects on resume parsing and ranking
* Proof-of-concept ATS (Applicant Tracking System)

---

## 📄 License

This project is open-source and free to use for non-commercial purposes. For commercial licensing, please contact the author.

---

## 🙏 Acknowledgements

* Developed by Amit Dashgupta as part of MSc Dissertation at Dublin Business School
* Special thanks to [spaCy](https://spacy.io), [Tesseract](https://github.com/tesseract-ocr/tesseract), [scikit-learn](https://scikit-learn.org), and [Kaggle](https://www.kaggle.com) for dataset resources
