Goal of the models: Accurately and consistently predict if a movie will have a average rating of greater than 6 

|index|Model|Test Accuracy|Test Precision|Test Recall|Test F1-score|Mean CV Accuracy|Std Dev CV Accuracy|
|---|---|---|---|---|---|---|---|
|0|SVM|0\.7718865598027127|0\.7956448911222781|0\.8828996282527881|0\.8370044052863436|0\.764103844471076|0\.00917934346949328|
|1|Decision Tree|0\.7262638717632552|0\.795880149812734|0\.7899628252788105|0\.792910447761194|0\.713231657440697|0\.013040825939252734|

Dataset Link: https://www.kaggle.com/datasets/alessandrolobello/the-ultimate-film-statistics-dataset-for-ml

Short highlights:
- SVM achieves the best held-out test performance (Accuracy ≈ 0.772, F1 ≈ 0.837).
- Decision Tree is competitive but shows lower generalization by cross-validation.
