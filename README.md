# Human Activity Recognition Project Report

## Project Summary

This project uses data from accelerometers on the belt, forearm, arm, and dumbbell of 6 participants to predict the **manner** ("classe" variable) in which exercises were performed. All other variables serve as predictors. The analysis describes preprocessing, Random Forest modeling, cross-validation, and predictions for the provided test cases.

---

## Methodology

- Data loaded from provided training and test sets.
- Irrelevant identifier and metadata columns removed.
- Both datasets were aligned to use common features only.
- Missing values were imputed using the mean.
- A Random Forest classifier was trained and accuracy was estimated with 5-fold cross-validation.
- The trained model was used to predict the exercise manner for 20 test cases in the quiz/test set.

---

## Results

- **Cross-validation accuracy:** 0.99
- **Expected out-of-sample error:** 0.01
- **Predicted classes for 20 test cases:**  
  `['B', 'A', 'B', 'A', 'A', 'E', 'D', 'B', 'A', 'A', 'B', 'C', 'B', 'A', 'E', 'E', 'A', 'B', 'B', 'B']`

---

## Discussion

The Random Forest algorithm was chosen for its robustness, strong accuracy, and ability to handle complex and noisy feature interactions. 5-fold cross-validation provided a reliable estimate for expected model error on unseen data. All results are reproducible, and the final output matches the requirements for peer review and quiz submission.

---

_This file, along with the HTML output, is prepared for submission and peer review as required._
