# Student Performance Prediction: Linear & Logistic Regression

A beginner-friendly machine learning notebook demonstrating two supervised learning models using Python and scikit-learn.

## What this notebook covers

### 1. Linear Regression — Marks Prediction
- Uses study hours as the input feature (`Study_Hour`).
- Predicts student marks (`Marks`).
- Splits the dataset into training and testing sets.
- Trains a `LinearRegression` model.
- Evaluates predictions using RMSE and R-squared.
- Accepts study hours from the user and predicts marks.
- Plots actual data, predicted values, and the user's prediction.

### 2. Logistic Regression — Pass/Fail Prediction
- Uses study hours as the input feature.
- Predicts the result: `0 = Fail`, `1 = Pass`.
- Splits the data into training and testing sets.
- Trains a `LogisticRegression` model.
- Evaluates the model using accuracy.
- Accepts study hours and displays the predicted result and pass probability.

## Project files

```text
Linear-Regression-Project/
├── Linear_Regression.ipynb
├── README.md
├── requirements.txt
└── student.csv              # Required for the Linear Regression section
```

## Dataset required

The Linear Regression section loads a file named `student.csv`. The CSV must contain these columns:

| Column | Description |
|---|---|
| `Study_Hour` | Number of hours studied |
| `Marks` | Student marks |

Place `student.csv` in the notebook's working directory, or upload it when the notebook prompts for a file.

The Logistic Regression section uses a small example dataset defined directly inside the notebook; it does not use `student.csv`.

## Run in Google Colab

The notebook currently uses `from google.colab import files` and `files.upload()`, so its upload cell is designed for Google Colab.

1. Open the notebook in Google Colab.
2. Run the first code cell.
3. When prompted, upload `student.csv`.
4. Follow the input prompts to enter study hours and view predictions.

## Run locally

Install the packages listed in `requirements.txt`.

The notebook's `google.colab` upload helper is specific to Google Colab. To run the first section in a local Jupyter environment, replace:

```python
from google.colab import files
upload = files.upload()
```

with a local CSV-loading line:

```python
df = pd.read_csv("student.csv")
```

Keep `student.csv` in the notebook's working directory.

## Install dependencies

```bash
pip install -r requirements.txt
```

## Important note

This is an educational demonstration with a small dataset and simple features. Its predictions should not be used to make real academic decisions. Reliable real-world predictions require representative data, appropriate validation, and careful consideration of additional factors.

## License

Add a license file if you want to specify the terms under which others may use, modify, or distribute this project.
