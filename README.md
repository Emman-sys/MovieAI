Goal of the models: Accurately and consistently predict if a movie will have a average rating of greater than 6 

|index|Model|Test Accuracy|Test Precision|Test Recall|Test F1-score|Mean CV Accuracy|Std Dev CV Accuracy|
|---|---|---|---|---|---|---|---|
|0|SVM|0\.7718865598027127|0\.7956448911222781|0\.8828996282527881|0\.8370044052863436|0\.764103844471076|0\.00917934346949328|
|1|Decision Tree|0\.7262638717632552|0\.795880149812734|0\.7899628252788105|0\.792910447761194|0\.713231657440697|0\.013040825939252734|

Dataset Link: https://www.kaggle.com/datasets/alessandrolobello/the-ultimate-film-statistics-dataset-for-ml

Short highlights:
- SVM achieves the best held-out test performance (Accuracy ≈ 0.772, F1 ≈ 0.837).
- Decision Tree is competitive but shows lower generalization by cross-validation.

## Project overview
This repository trains and evaluates classifiers to predict whether a movie's average rating will exceed 6. It includes preprocessing, model training, cross-validation, and reporting of standard classification metrics.

## Quick start / Usage
- Clone the repo and install dependencies (typical Python stack: pandas, scikit-learn, joblib, etc.).
- Place the downloaded Kaggle dataset in the data/ directory or update the data path in the notebook/script(I did this in Google Collab so for best results or if you dont feel like coding just upload the entire repo to your drive then get the path to the icluded dataset and edit the second cell).
- Run the training script or notebook to reproduce preprocessing and model runs:
  - Example (from repo root): python train.py --data data/movies.csv
  - Or open the provided notebook(s) for an interactive run.
  - Note: the dataset included in this repository's data/ directory is already cleaned for the experiments — director_names entries with "-" were purged.

## Evaluation summary
- Primary metric used: F1-score (balance between precision and recall).
- Cross-validation reported to evaluate generalization (mean and std dev shown above).
- Best model on held-out test set: SVM (highest F1 and Accuracy in the table).

## Contributing
Contributions, bug reports and feature requests are welcome. Please open an issue or submit a PR with a clear description of changes.

## License
This project is released under the MIT License. See the LICENSE file for details.
