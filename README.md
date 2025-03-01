# Crop Recommendation Models

This project implements various machine learning models to predict the best crop to plant based on environmental conditions and soil characteristics. The dataset used for this project is `Crop_recommendation.csv`.

## Libraries Used

- `pandas`: For data manipulation and analysis.
- `numpy`: For numerical operations.
- `matplotlib`: For data visualization.
- `seaborn`: For enhanced data visualization.
- `scikit-learn`: For machine learning algorithms and model evaluation.
- `xgboost`: For the XGBoost classifier.

## Dataset

The dataset contains features related to soil and environmental conditions, along with a target variable representing the recommended crop. The target variable is encoded using `LabelEncoder`.

## Models Implemented

The following machine learning models are implemented in this project:

1. **Random Forest Classifier (RF)**
2. **Gradient Boosting Classifier (GB)**
3. **AdaBoost Classifier (AB)**
4. **XGBoost Classifier (XGB)**

## Model Training and Evaluation

The dataset is split into training and testing sets (80% train, 20% test). Each model is trained on the training set and evaluated on both the training and testing sets. The accuracy scores are printed for each model, along with cross-validation scores.

### Results

The following accuracies were obtained for each model:

| Model | Train Accuracy | Test Accuracy | Cross Validation Score |
|-------|----------------|----------------|------------------------|
| RF    | 99.77          | 99.77          | 99.77                  |
| GB    | 99.09          | 99.09          | 99.09                  |
| AB    | 17.27          | 17.27          | 17.27                  |
| XGB   | 99.31          | 99.31          | 99.31                  |

## Visualizations

The accuracies of the models are visualized using bar plots and line plots.

### Bar Plot

![Bar Plot of Model Accuracies](bar_plot.png)

### Line Plot

![Line Plot of Model Accuracies](line_plot.png)

## Conclusion

The Random Forest and XGBoost classifiers performed exceptionally well, achieving high accuracy scores. The AdaBoost classifier, however, did not perform well in this scenario. Further tuning and feature engineering may improve the performance of the models.

## How to Run

1. Clone the repository.
2. Install the required libraries using `pip install -r requirements.txt`.
3. Place the `Crop_recommendation.csv` file in the same directory.
4. Run the script to train the models and visualize the results.

## License

This project is licensed under the MIT License.
