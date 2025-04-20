# Movie-Genre-Classification
A machine learning project to classify movies into genres based on their plot summaries. The project involves text preprocessing, feature extraction using NLP techniques, and evaluating multiple classifiers to build an accurate genre prediction model.

## 📂 Dataset

The dataset consists of three `.txt` files:

- `train_data.txt` – Movie plot descriptions with genres (for training)
- `test_data.txt` – Movie plot descriptions (for testing/prediction)
- `test_data_solution.txt` – Ground truth genres for test data (for evaluation)

Due to GitHub file size restrictions, these files are not stored directly in this repository.

### 🔗 How to Access the Dataset

The dataset is stored in a public Google Drive folder:

[👉 Download Dataset from Google Drive]([https://drive.google.com/your-shared-link-here](https://drive.google.com/drive/folders/1xTriIeW9Qjun1ywSCLQ6ebsi5DS6clWo?usp=sharing))

> Alternatively, in Google Colab, you can load the data using Google Drive mount or `gdown`:

```python
# Option 1: Mount Google Drive
from google.colab import drive
drive.mount('/content/drive')

# Option 2: Use gdown (replace file_id with actual ID)
!pip install gdown
!gdown --id your_file_id_here
