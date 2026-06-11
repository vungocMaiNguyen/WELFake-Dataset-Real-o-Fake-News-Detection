# WELFake-Dataset-Real-o-Fake-News-Detection

The project was developed as part of the Digital Transformation Management course at the University of Bologna.

It aims to predict whether a news article is *Fake* or *Real* using the article title and full text. The task is treated as a supervised binary classification problem based on the WELFake Dataset.

Label convention used in the notebook:

- 0 = Fake
- 1 = Real

## Open the Notebook in Google Colab

Click the button below to launch the project directly in Google Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1fNOxDDH3228_xxHm_VwxuhGFMSqMLnUU#scrollTo=UIVDzO2mSBTQ)

## Required Dataset

The project uses the [WELFake Dataset](https://www.kaggle.com/datasets/saurabhshahane/fake-news-classification), a fake news classification dataset containing news titles, article texts, and binary labels.

The dataset CSV is not included in this repository for size reasons.

The notebook expects the file to be named:

text
WELFake_Dataset.csv


## How to Use It in Colab

### Option 1: Upload the CSV directly in Colab

1. Download WELFake_Dataset.csv from Kaggle.
2. Open the notebook in Google Colab.
3. Upload the file in the Colab session, or place it inside a data/ folder.

The notebook automatically checks these paths:

text
WELFake_Dataset.csv
data/WELFake_Dataset.csv
/content/WELFake_Dataset.csv
/content/data/WELFake_Dataset.csv


### Option 2: Use Google Drive

1. Download WELFake_Dataset.csv once from Kaggle.
2. Upload the file into your Google Drive.
3. Recommended path:

text
MyDrive/Colab Notebooks/data/WELFake_Dataset.csv


4. Mount Google Drive in Colab and copy the dataset to the path expected by the notebook:

python
from google.colab import drive
drive.mount('/content/drive')

!mkdir -p /content/data
!cp "/content/drive/MyDrive/Colab Notebooks/data/WELFake_Dataset.csv" "/content/data/WELFake_Dataset.csv"


After this step, run the notebook cells from the beginning.
