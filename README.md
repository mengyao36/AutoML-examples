# AutoML-examples

## Dataset Selected
- SPARCS

## Two experiments created using autoML package `mljar-supervised`
- Experiment 1:
  - DV: Type of admission (multiclass var)
  - Best model: Xgboost
  - Log-loss:  0.22 (79% better than baseline)
  - AUC: ? not sure how to report this value for multiclass var, output as below
|       |   Elective |   Emergency |    Newborn |   Not Available |   Trauma |     Urgent |   accuracy |   macro avg |   weighted avg |   logloss |
|:----------|-----------:|------------:|-----------:|----------------:|---------:|-----------:|-----------:|------------:|---------------:|----------:|
| precision |   0.826797 |    0.961089 |   0.993023 |        1        |     1    |   0.768595 |   0.925859 |    0.924918 |       0.92445  |  0.222508 |
| recall    |   0.898225 |    0.967937 |   0.997664 |        0.8      |     0.25 |   0.568807 |   0.925859 |    0.747106 |       0.925859 |  0.222508 |
| f1-score  |   0.861032 |    0.964501 |   0.995338 |        0.888889 |     0.4  |   0.653779 |   0.925859 |    0.793923 |       0.923138 |  0.222508 |
| support   | 845        | 2807        | 428        |        5        |    12    | 327        |   0.925859 | 4424        |    4424        |  0.222508 |
- Experiment 2: 
  - DV: Total charges (continuous var)
  - Best model: Xgboost
  - Log-loss: 0.22 (79% better than baseline)
