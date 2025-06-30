# Random-Forest-classifier-with-SHAP-explanations-on-RDF-derived-data.

## Project Overview
A machine learning project using a Random Forest classifier trained on RDF-derived data with SHAP explanations for model interpretability.

## Main Files

- `tabular_training_testing.ipynb`  
  Contains the main pipeline for conversion into tabular data, training, testing, evaluation and explaining the Random Forest classifier using SHAP.

- `strategy2a,analysis.ipynb`  
  Handles RDF data analysis using SPARQL.

## Project Overview
- Loaded RDF DATA from aifbfixed_complete.n3 to extract features for entities in trainingSet.tsv and testSet.tsv.
- Each literal features and labels for each entity were encoded.
- Trained a Random Forest classifier on encoded literal features of entities of the traininSet.tsv and its corresponding encoded labels.
- Tested the model on the encoded features of the testSet.tsv
- Evaluated model performance on a labeled test set.
- Explained predictions using SHAP summary plots and force plots.
- Analysis of the RDF dataset using SPARQL queries.

## Files Included
- `aifbfixed_complete.n3` – RDF dataset including features for each entity of the dataset.
- `trainingSet.tsv`, `testSet.tsv` – Training and test splits.
- `completeDataset.tsv`  - All entities of the trainingSet.tsv and testSet.tsv including their labels.
- `tabular_training_testing.ipynb` - Includes conversion of the rdf dataset into tabular form, feature encoding, training, testing, evaluation and interpretation of the model using SHAP.
- `strategy2a,analysis.ipynb` - Analysis of the rdf data set using SPARQL.
- `rf_model.pkl` - Saving the model.
- `README.md` – Project documentation.

## Example Output
- SHAP summary plots for global feature importance.
- SHAP force plots for individual instance-level explanations.
- Precision, recall, f1 score, support for each classification label including accuracy, macro average and weighted average using classification report of sklearn
- Predicted encoded labels for each instance of the testSet.tsv.

## Requirements
- Python 3.10.18 version
- ipykernel
- pandas
- rdflib
- scikit-learn
- shap
- matplotlib
# Node.js must be installed separately for SHAP interactive plots, (conda install -c conda-forge nodejs if done using conda prompt)
- ipywidgets  # Required for SHAP interactive plots in Jupyter
