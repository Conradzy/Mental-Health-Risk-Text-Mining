# Mental Health Risk Text Mining

Analyzes mental-health posts across five risk levels, from no risk to very high risk. It combines text preprocessing, VADER sentiment, TF-IDF classification, feature interpretation, and LDA topic modeling.

## Workflow

1. Load and clean `mentalhealth.csv` text and risk labels.
2. Preprocess posts with tokenization and normalization.
3. Analyze VADER sentiment overall and by risk category.
4. Train a class-balanced TF-IDF Logistic Regression classifier.
5. Inspect discriminative terms and discover topics with LDA.

## Data Requirements

- `mentalhealth.csv` with a text field and numeric target from 0 to 4.

Datasets and generated artifacts are not included unless they are embedded directly in the notebook.

## Requirements

- pandas
- NumPy
- scikit-learn
- NLTK
- VADER Sentiment
- gensim
- Matplotlib
- Seaborn

Install missing packages in your Jupyter or Google Colab environment before running the notebook.

## Running the Notebook

1. Open [`textminingfinals.ipynb`](textminingfinals.ipynb) in Jupyter Notebook or Google Colab.
2. Place any required data files in the path expected by the notebook.
3. Update local or Google Drive paths where needed.
4. Run the cells from top to bottom.

## Outputs

- Risk-distribution and sentiment charts
- Classification report and confusion matrix
- Top TF-IDF terms by class
- LDA topic visualization
- Summary metrics

## Security and Responsible Use

This notebook is for research and education. Its predictions are not medical diagnoses and should not be used as a substitute for qualified professional assessment.

## Repository Contents

```text
.
|-- README.md
`-- textminingfinals.ipynb
```

## Notes

- This repository preserves the analysis as a notebook-first educational project.
- Results may vary with dataset versions, random splits, package versions, and available hardware.
- Review file paths and runtime-specific commands before executing outside Google Colab.
