### **Stock Price Prediction with LSTM**
This project demonstrates how to use an LSTM (Long Short-Term Memory) neural network to predict stock prices based on historical data. The code loads, preprocesses, and scales stock data, builds and trains an LSTM model, and evaluates its performance.

**Requirements**
To run this code, you'll need the following Python packages:

- `gdown` for downloading files from Google Drive
- `pandas` for data manipulation
- `numpy` for numerical operations
- `scikit-learn` for data scaling
- `matplotlib` for plotting
- `tensorflow` for building the LSTM model

**Usage**
1. Data Download: The code downloads a CSV file from Google Drive using gdown.
2. Data Preprocessing:
* It loads the dataset, selects Open and Close columns, and scales the data using MinMaxScaler.
* The data is then split into training and testing sets.
3. LSTM Model:
* A Sequential LSTM model with two LSTM layers and two dense layers is created.
* The model is trained on the training data to minimize mean squared error.
4. Model Evaluation: The model’s performance is evaluated using RMSE (Root Mean Square Error).
  
**How to Run**
Simply execute the code cells in sequence in a Jupyter Notebook or Google Colab.

After training, the model will output RMSE, indicating the model's accuracy. You can adjust parameters like epochs or batch_size to optimize model performance.
