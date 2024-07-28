# Wine Quality Predictor

This project is a basic Wine Quality Predictor using a Random Forest Classifier. The model is trained on the `winequality-red.csv` dataset, which includes various features related to the properties of red wine. The project involves data visualization, preprocessing, and building a machine learning model to predict the quality of wine.

## Project Structure

- `wine-predictor.py`: Main script containing the code for data visualization, preprocessing, and model training.
- `winequality-red.csv`: Dataset containing various properties of red wine.

## Data Visualization

The project includes various data visualizations to explore the relationships between wine quality and its properties. The visualizations are created using Seaborn and Matplotlib:

- Count plot of wine quality distribution.
- Bar plots of wine quality vs. various properties such as volatile acidity, fixed acidity, citric acid, residual sugar, chlorides, total sulfur dioxide, free sulfur dioxide, pH, density, sulphates, and alcohol.

## Model Training and Evaluation

The model is built using a Random Forest Classifier from the `sklearn` library. The steps involved are:

1. Load and inspect the dataset.
2. Visualize the data.
3. Drop irrelevant features (`pH` and `density`).
4. Split the data into training and testing sets.
5. Train the Random Forest Classifier.
6. Evaluate the model using R2 score and accuracy score.

## Results

The model's performance is evaluated on the test data, and the following metrics are printed:

- Error Score (R2 score)
- Test Accuracy

```python
print('Error Score : ', error_accuracy)
print('Test Accuracy : ', test_accuracy)
