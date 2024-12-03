# Model Card

For additional information see the Model Card paper: https://arxiv.org/pdf/1810.03993.pdf

## Model Details
This model uses the RandomForest Classifier.

## Intended Use
The model is used to determine whether an individual makes above or below $50,000 per year.
## Training Data
The training data contains columns based on items such as marital status, occupation, sex, salary, and other factors.
## Evaluation Data
The training data is sliced down to a smaller table using the same features, roughly 1/4 of the size of the original.
## Metrics
Precision: 0.7529 | Recall: 0.6349 | F1: 0.6889

## Ethical Considerations
If used to determine something such as eligibility for loans or mortgages, could discriminate against individuals based on race, education and other factors. 

## Caveats and Recommendations
This data is old, and does not account for changes in potential rises in income. Also, while RandomForestClassifier can be accurate, it can suffer from overfitting, which can influence new data.
