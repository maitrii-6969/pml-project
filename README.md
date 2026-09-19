# pml-project
# Predicting How Well Barbell Lifts Are Performed

Course project for Practical Machine Learning.

Using accelerometer data from the belt, forearm, arm and dumbbell of 6 participants, this project predicts the manner in which a barbell lift was performed (the `classe` variable, A to E).

**View the report online:** https://maitrii-6969.github.io/pml-project/

## Files
- `pml_report.Rmd`: R Markdown source with all the code
- `index.html`: compiled HTML report (the page linked above)

## Approach
- Cleaned the data (removed identifier columns, mostly-empty columns and near-zero-variance predictors)
- Held out 30% of the data as a validation set
- Fitted a baseline decision tree and a random forest with 5-fold cross-validation
- Estimated the out-of-sample error on the validation set
- Predicted the 20 test cases with the random forest

## Data source
Velloso, E., Bulling, A., Gellersen, H., Ugulino, W., Fuks, H. *Qualitative Activity Recognition of Weight Lifting Exercises.* Proceedings of the 4th International Conference in Cooperation with SIGCHI (Augmented Human '13), Stuttgart, 2013. http://web.archive.org/web/20161224072740/http:/groupware.les.inf.puc-rio.br/har
