# Machine Learning with Python

Python is a popular language for machine learning due to its simplicity and extensive libraries.

## Key Libraries
- **Scikit-learn**: Provides simple and efficient tools for data mining and data analysis.
- **Pandas**: Offers data structures and data analysis tools.
- **NumPy**: Supports large, multi-dimensional arrays and matrices.

## Steps
1. **Data Preparation**: Load and preprocess your data.
2. **Model Selection**: Choose an appropriate model for your problem.
3. **Training**: Train your model using training data.
4. **Evaluation**: Assess the model’s performance using test data.

## Example Code
### Python: Simple Linear Regression
```python
from sklearn.linear_model import LinearRegression
from sklearn.model_selection import train_test_split
from sklearn.metrics import mean_squared_error

# Example data
X = [[1], [2], [3], [4]]
y = [1, 4, 9, 16]

# Split data
X_train, X_test, y_train, y_test = train_test_split(X, y, test_size=0.2)

# Train model
model = LinearRegression()
model.fit(X_train, y_train)

# Predict and evaluate
y_pred = model.predict(X_test)
print(f'Mean Squared Error: {mean_squared_error(y_test, y_pred)}')
```

## Learning Resources

- [Python Machine Learning - YouTube](https://www.youtube.com/watch?v=7eh4d6sabA0)
- [Scikit-learn Documentation](https://scikit-learn.org/stable/)

## Next Steps

1. Experiment with different models and datasets.
2. Work on machine learning projects to build a portfolio.
