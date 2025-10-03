# Customer Churn Prediction with ANN

This project demonstrates the process of building an Artificial Neural Network (ANN) for predicting customer churn in a bank using Python and Keras. The workflow covers the end-to-end process of data preprocessing, model building, training, evaluation, and making predictions for new observations.

## Dataset

The notebook uses the `Churn_Modelling (1).csv` dataset, which contains information about bank customers, including features such as:

- Credit Score
- Geography
- Gender
- Age
- Tenure
- Balance
- Number of Products
- Has Credit Card
- Is Active Member
- Estimated Salary
- Exited (target variable, 1 = churned, 0 = stayed)

## Project Structure

- **Data Import**: Loads the dataset and displays a preview.
- **Preprocessing**:
  - Encoding categorical features (`Geography`, `Gender`) using one-hot encoding.
  - Feature scaling using `StandardScaler`.
  - Splitting the dataset into training and test sets.
- **Model Building**:
  - Initializes a Sequential ANN with Keras.
  - Adds two hidden layers and an output layer.
  - Compiles the model with Adam optimizer and binary crossentropy loss.
- **Training**: Trains the ANN on the training set.
- **Evaluation**:
  - Predicts on the test set.
  - Computes and visualizes the confusion matrix.
- **Single Prediction**: Predicts whether a new customer (with provided details) will leave the bank.

## Key Libraries Used

- `numpy` and `pandas` for data handling
- `scikit-learn` for preprocessing, splitting, and metrics
- `keras` (TensorFlow backend) for building and training the ANN
- `matplotlib` and `seaborn` for visualization

## Usage

1. **Clone the repository** and ensure you have the required dataset (`Churn_Modelling (1).csv`).
2. **Install dependencies** (if using Colab, most are pre-installed):

   ```bash
   pip install numpy pandas scikit-learn matplotlib seaborn keras
   ```

3. **Open and run the notebook** (`Untitled2.ipynb`) step by step.

## Example: Predicting New Customer Churn

The notebook includes a sample for predicting if a new customer will churn, using the same preprocessing and model as the main workflow. Update the customer details in the code cell to predict for different scenarios.

## Confusion Matrix

A confusion matrix is generated to visualize the model's performance on the test set.

## Notes

- Ensure the dataset path is correct in the notebook.
- The ANN hyperparameters (layers, units, epochs, batch size) can be tuned for better performance.
- The notebook is structured for Google Colab, but can run in any Jupyter environment with the required dependencies.

## License

This project is for educational purposes.
