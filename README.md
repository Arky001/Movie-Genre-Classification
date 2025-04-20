```
# Movie-Genre-Classification

A machine learning project to classify movies into genres based on their plot summaries.  
This involves text preprocessing, feature extraction using NLP techniques, and experimenting with multiple classification algorithms to build a robust genre prediction model.

---

## 📂 Dataset

The dataset consists of three `.txt` files with the following format:

### Train Data (`train_data.txt`)
```
ID ::: TITLE ::: GENRE ::: DESCRIPTION
```

### Test Data (`test_data.txt`)
```
ID ::: TITLE ::: DESCRIPTION
```

### Test Solution (`test_data_solution.txt`)
```
ID ::: GENRE
```

> **Note**: Due to GitHub's file size limitations, the dataset files are not included in this repository.

---

## 🔗 Access the Dataset

The dataset is stored in a public Google Drive folder:  
[👉 Access Dataset on Google Drive](https://drive.google.com/drive/folders/1xTriIeW9Qjun1ywSCLQ6ebsi5DS6clWo?usp=sharing)

To use the dataset in **Google Colab**, you can mount your Google Drive:

```python
from google.colab import drive
drive.mount('/content/drive')
```

---

## 🧠 Project Workflow

1. **Data Loading**  
   Read the `.txt` files using `pandas.read_csv()` with a custom separator (`:::`).

2. **Preprocessing**  
   - Clean text: lowercase, remove special characters, etc.
   - Vectorize using TF-IDF
   - Encode multi-label genres with `MultiLabelBinarizer`

3. **Model Training**  
   Tried and evaluated multiple classifiers:
   - Logistic Regression
   - Multinomial Naive Bayes
   - Random Forest Classifier

4. **Evaluation**  
   Compared models using classification metrics like accuracy and F1-score.

5. **Prediction**  
   Applied the best-performing model on the test data.

---

## 🚀 How to Run (Google Colab Recommended)

1. Open the project notebook in Google Colab.
2. Mount Google Drive to access the dataset.
3. Follow the code cells to:
   - Load and preprocess data
   - Train and evaluate models
   - Predict genres for the test set

---

## ✅ Output

- Final predictions saved to `submission.csv`
- Test samples labeled with predicted genres

---

## 📌 Credits

Dataset Source:  
ftp://ftp.fu-berlin.de/pub/misc/movies/database/

---

Feel free to fork, use, or improve this project. Contributions are welcome!
```
