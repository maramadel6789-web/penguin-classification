
# Penguin Species Classification

A machine learning lab that explores the penguins dataset and trains multiclass classification models to predict a penguin's species from its physical measurements.

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/maramadel6789-web/penguin-classification/blob/main/Multiclass_Classification_Penguins_Lab.ipynb)

## Overview

The notebook `Multiclass_Classification_Penguins_Lab.ipynb` walks through a complete multiclass classification workflow:

1. **Explore the data** – load the dataset and map numeric labels to species names.
2. **Clean the data** – find and remove rows with missing values.
3. **Analyze features** – use box plots to see how each feature differs by species.
4. **Prepare the data** – split into training (70%) and test (30%) sets, using stratification to keep the class proportions.
5. **Train a Logistic Regression model** – a multiclass classifier with scikit-learn.
6. **Evaluate the model** – classification report, accuracy, precision, recall, confusion matrix, and ROC curves with AUC (One vs Rest).
7. **Use a pipeline** – scale the features and train a Support Vector Machine (SVM).
8. **Save and reuse the model** – save the trained model with joblib and predict the species of new penguins.

## Dataset

`penguins.csv` contains measurements of three penguin species:

| Column | Description |
|---|---|
| `CulmenLength` | Length of the culmen (bill) in mm |
| `CulmenDepth` | Depth of the culmen in mm |
| `FlipperLength` | Length of the flipper in mm |
| `BodyMass` | Body mass in grams |
| `Species` | **Label** – 0 = Adelie, 1 = Gentoo, 2 = Chinstrap |

**Citation:** The penguins dataset is a subset of data collected and made available by Dr. Kristen Gorman and the Palmer Station, Antarctica LTER, a member of the Long Term Ecological Research Network.

## Repository Contents

- `Multiclass_Classification_Penguins_Lab.ipynb` – the lab notebook, with a short explanation above each code cell
- `penguins.csv` – the dataset

## Requirements

- Python 3
- pandas
- numpy
- matplotlib
- scikit-learn
- joblib

Install them with:

```bash
pip install pandas numpy matplotlib scikit-learn joblib
```

## How to Run

1. Clone or download this repository.
2. Make sure `penguins.csv` is in the same folder as the notebook.
3. Open the notebook in Jupyter Notebook, JupyterLab, or Google Colab (if using Colab, upload `penguins.csv` to the session first).
4. Run the cells from top to bottom.

## Evaluation Metrics

- **Accuracy** – the share of predictions that are correct.
- **Precision** – of the penguins predicted as a species, how many truly belong to it.
- **Recall** – of the penguins that truly belong to a species, how many were found.
- **Confusion matrix** – shows predicted vs. actual species for each class.
- **ROC / AUC** – measures how well the model separates each species from the rest (One vs Rest).
