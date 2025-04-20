# 🎬 Movie Genre Classification

A machine learning project to classify movies into genres based on their plot summaries.  
It includes text preprocessing, NLP-based feature extraction, and experimenting with multiple classifiers to build a robust prediction model.

---

## 📂 Dataset Format

The dataset consists of three `.txt` files in the following formats:

### 🧾 Train Data (`train_data.txt`)
```
ID ::: TITLE ::: GENRE ::: DESCRIPTION
```

### 🧾 Test Data (`test_data.txt`)
```
ID ::: TITLE ::: DESCRIPTION
```

### 🧾 Test Solution (`test_data_solution.txt`)
```
ID ::: GENRE
```

> **Note:** Due to GitHub’s file size limits, the dataset is not directly included in the repository.

---

## 🔗 Access the Dataset

The dataset is available on Google Drive:  
[📥 Click to Access Dataset](https://drive.google.com/drive/folders/1xTriIeW9Qjun1ywSCLQ6ebsi5DS6clWo?usp=sharing)

To use the dataset in **Google Colab**, mount your Google Drive:

```python
from google.colab import drive
drive.mount('/content/drive')
```

---

## 🛠️ Project Workflow

### 1. **Data Loading**
- Load `.txt` files using `pandas.read_csv()` with a custom separator (`:::`).

### 2. **Text Preprocessing**
- Convert text to lowercase
- Remove special characters and stopwords
- Tokenize and clean descriptions

### 3. **Feature Extraction**
- Use **TF-IDF Vectorization** for text features
- Encode multi-label genres using `MultiLabelBinarizer`

### 4. **Model Training**
- Train and evaluate various models:
  - Logistic Regression
  - Multinomial Naive Bayes
  - Random Forest Classifier

### 5. **Evaluation**
- Metrics: Accuracy, Precision, Recall, F1-score

### 6. **Prediction**
- Predict genres for test data
- Save final output to `submission.csv`

---

## 🚀 How to Run (Recommended in Google Colab)

1. Upload the `.txt` files or mount your Google Drive
2. Run the notebook step-by-step:
   - Load & preprocess data
   - Train and evaluate models
   - Predict and save results

---

## ✅ Output

- A `submission.csv` file with format:
```
ID,Predicted Genres
1,drama
2,thriller
3,comedy|romance
```

---

## 📌 Credits

**Dataset Source:**  
ftp://ftp.fu-berlin.de/pub/misc/movies/database/

---

## 🤝 Contributions

Feel free to fork, use, or contribute to this project. PRs are welcome!
