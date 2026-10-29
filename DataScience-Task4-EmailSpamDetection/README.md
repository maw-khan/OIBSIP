# Email Spam Detection

A machine-learning project that classifies Emails as **spam** or **ham** (legitimate messages). The notebook covers data exploration, TF-IDF feature extraction, model training, evaluation, predictions, and saving a reusable pipeline.

## Project Features

- Dataset inspection and cleaning
- Stratified training/test split
- TF-IDF text feature extraction
- Comparison of Multinomial Naive Bayes, Logistic Regression, and Linear SVM
- Accuracy, spam precision, spam recall, and spam F1-score
- Classification report and confusion matrix
- Example predictions on new messages
- Export of the selected model pipeline with Joblib

## Project Structure

```text
Email-Spam-Detection/
├── Email_Spam_Detection.ipynb
├── requirements.txt
├── README.md
└── .gitignore
```

The notebook creates `email_spam_detection_pipeline.joblib` when its final model-saving cell is run. This generated file is excluded from version control by default.

## Requirements

- Python 3.10 or newer recommended
- Internet access to download the dataset on the first run

## Setup

### 1. Clone the repository

```bash
git clone [https://github.com/maw-khan/SMS-Spam-Detection.git](https://github.com/maw-khan/OIBSIP/
cd DataScience-Task4-EmailSpamDetection
```

### 2. Create and activate a virtual environment

Windows PowerShell:

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

If PowerShell blocks activation, use Command Prompt instead:

```bat
.venv\Scripts\activate.bat
```

### 3. Install dependencies

```bash
python -m pip install -r requirements.txt
```

### 4. Open the notebook

Open `Email_Spam_Detection.ipynb` in VS Code or Jupyter Notebook, select the environment created above as the kernel, and run the cells from top to bottom.

## Dataset

The notebook loads a tab-separated Email spam dataset from a public GitHub repository. An internet connection is required for the initial download. Refer to the dataset source linked in the notebook for its provenance and terms.

## Evaluation

The notebook compares models using:

- **Accuracy:** overall fraction of correct predictions
- **Spam precision:** fraction of messages predicted as spam that are spam
- **Spam recall:** fraction of actual spam messages detected
- **Spam F1-score:** harmonic mean of spam precision and recall

Because legitimate messages are more common than spam in this dataset, accuracy alone is not sufficient to assess performance.

## Limitations

- Results depend on the dataset and train/test split.
- The dataset may not represent current scam messages, new spam tactics, or all languages.
- This is a learning project, not a production-grade spam filter. Review false positives and false negatives before using a model in a real messaging system.

## Technologies

Python · pandas · scikit-learn · TF-IDF · Matplotlib · Seaborn · Joblib
