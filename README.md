# SVM Classifier for Artificial Muscle Classification

## Overview
This repository contains a Support Vector Machine (SVM) based approach for classifying use cases of artificial muscles, addressing the challenge of feature selection in sparse datasets. The project includes multiple machine learning models, each tailored to work with different preprocessing strategies.

## Repository Structure

### SVM Models
- `bivariate_svm`: Contains 10 bivariate SVM models. Each model is trained using a unique pair of features from the dataset to ensure maximum utilization of non-null data points.

### Neural Network Models
- `nn_raw`: A neural network model trained on the original dataset with missing values filled with zeros. [Current accuracy: 32%]
- `nn_imputed`: A neural network model trained on data imputed using the imputation tools from SciKit Learn. [Current accuracy: 59%]
- `nn_augmented`: A neural network model trained on data augmented with actual values obtained from reliable sources. [Current accuracy: 75%]

### Datasets
- `nn_raw/data/original_data.csv`: The original dataset as provided.
- `nn_imputed/data/new_data.csv`: The dataset after applying imputation techniques to handle missing values.
- `nn_augmented/data/augmented_data.csv`: The dataset post data augmentation to address the issue of missing information.

## Resources
- For a comprehensive understanding of the project, consult the `final_report.pdf`.
- For a quick overview and project insights, refer to the `final_presentation.pdf`.

## Access and Usage
Each folder within this repository is self-contained, with its own dataset and a Jupyter Notebook (`*.ipynb`) detailing the code and methodology used.

Feel free to delve into the models and datasets provided, and refer to the documentation for a deeper insight into the project's scope and methodologies.

