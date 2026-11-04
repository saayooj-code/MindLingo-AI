# MindLingo-AI
MindLingo AI is a multilingual NLP and deep learning project that classifies text-based emotional experiences in English, Malayalam, and Manglish using multilingual BERT. It features an interactive Gradio interface for text classification and explores AI-powered multilingual language analysis for educational and research purposes.


# 🧠 MindLingo AI

### Bridging Languages. Understanding Emotional Expression.

**MindLingo AI** is a multilingual NLP and deep learning project that classifies text-based emotional experiences in **English, Malayalam, and Manglish**.

The project uses a fine-tuned multilingual BERT model and a Gradio interface to demonstrate multilingual text classification.

---

## 🌟 Features

* 🌐 **Multilingual Support:** English, Malayalam, and Manglish.
* 🧠 **Deep Learning:** Uses a pretrained multilingual BERT model.
* 💬 **Text Classification:** Classifies text into four predefined categories.
* 📊 **Model Evaluation:** Evaluates performance using accuracy, precision, recall, F1-score, and a confusion matrix.
* 🖥️ **Interactive Interface:** Provides a simple web interface using Gradio.
* 🔍 **Prediction Confidence:** Displays the model's confidence scores for its predicted categories.

## 🎯 Project Objectives

* Explore multilingual text classification using NLP.
* Apply deep learning to text written in different languages and scripts.
* Investigate how multilingual transformer models perform on English, Malayalam, and Manglish text.
* Develop an interactive demonstration using Gradio.
* Promote responsible and privacy-conscious AI development.

## 🏷️ Classification Categories

| Label               | Description                                              |
| ------------------- | -------------------------------------------------------- |
| `GENERAL_WELLBEING` | Text expressing general or positive everyday experiences |
| `STRESS_RELATED`    | Text expressing stress-related experiences               |
| `LOW_MOOD`          | Text expressing low mood                                 |
| `MIXED_EXPERIENCES` | Text containing a combination of experiences             |

These categories are dataset labels, not clinical assessments or mental health diagnoses.

## 🛠️ Technologies Used

* Python
* Pandas and NumPy
* Matplotlib and Seaborn
* Scikit-learn
* Hugging Face Transformers
* PyTorch
* Gradio
* Google Colab

## 📂 Project Structure

```text
mindlingo-ai/
├── notebooks/
│   └── MindLingo_AI_Training.ipynb
├── dataset/
│   └── README.md
├── app.py
├── requirements.txt
├── README.md
├── .gitignore
└── LICENSE
```

*Note: This is a suggested structure. Add files as they are created.*

## 📊 Dataset

The project expects a labelled CSV dataset named:

`student_mental_wellbeing_multilingual.csv`

### Required columns

| Column             | Description                     |
| ------------------ | ------------------------------- |
| `text`             | Text sample for classification  |
| `language`         | English, Malayalam, or Manglish |
| `experience_label` | Target classification label     |

The dataset should contain sufficiently diverse and accurately labelled examples from all supported languages.

Use appropriately licensed public data or consent-based data collection. Remove identifying information and avoid publishing sensitive text. Do not present synthetic examples as real participant responses.

## ⚙️ Model

MindLingo AI uses **`bert-base-multilingual-cased`**, a pretrained multilingual BERT model.

The model is fine-tuned on the labelled dataset to perform four-class text classification.

### Workflow

1. Load the dataset.
2. Clean and validate the text.
3. Explore the dataset and label distribution.
4. Encode labels and tokenize text.
5. Split the data into training, validation, and test sets.
6. Fine-tune the multilingual BERT model.
7. Evaluate performance on held-out test data.
8. Demonstrate predictions using Gradio.

## 📈 Evaluation Metrics

Model performance is assessed using:

* Accuracy
* Precision
* Recall
* Macro F1-score
* Confusion matrix

Actual evaluation results should be added after training. Performance may differ across languages, particularly if the dataset is imbalanced or contains limited Manglish examples.

## 🚀 Getting Started

### Option 1: Google Colab

1. Open your training notebook in Google Colab.
2. Install the required Python libraries.
3. Upload `student_mental_wellbeing_multilingual.csv`.
4. Run the notebook cells in order.
5. Evaluate the trained model.
6. Launch the Gradio demonstration.

### Option 2: Run Locally

Clone the repository:

```bash
git clone https://github.com/YOUR_USERNAME/mindlingo-ai.git
cd mindlingo-ai
```

Create a virtual environment and install dependencies:

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

Install the dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python app.py
```

*Note: Local execution requires a compatible `app.py`, trained model files or model-loading configuration, and a suitable dataset/model setup.*

## 🔮 Future Improvements

* Improve Manglish text normalization.
* Expand the dataset with diverse language samples.
* Evaluate classification performance separately for each language.
* Compare multilingual transformer architectures.
* Improve handling of ambiguous and mixed-language text.
* Add model cards and documentation about dataset limitations.

## 🔒 Responsible AI & Limitations

MindLingo AI is an educational and research demonstration. It classifies text according to predefined dataset categories; it cannot reliably determine a person's actual emotional state or diagnose mental health conditions.

Predictions may be inaccurate due to sarcasm, context, spelling variations, code-switching, or limitations in the training data. Confidence scores are model estimates, not probabilities that a person has a particular mental health condition.

Avoid submitting private or sensitive personal information to publicly hosted demonstrations. Obtain appropriate consent and approvals before collecting student data, particularly from minors.

## 👨‍💻 Author

**Your Name:** Add your name here
**Project:** MindLingo AI
**Domain:** Data Science | NLP | Deep Learning

## 📄 License

Choose a suitable open-source license, such as the MIT License, if you have the rights to distribute your code and any included assets or data. A code license does not automatically grant rights to redistribute a dataset or pretrained model.

---

⭐ If you find this project interesting, consider starring the repository!
