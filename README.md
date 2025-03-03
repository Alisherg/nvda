# Stock Price Movement Prediction for NVDA

## Project Overview
This project aims to predict whether NVIDIA Corporation's (NVDA) stock closing price will increase the next day. Using historical price data and technical indicators (such as daily return and deviation from the 10-day simple moving average), this task is approached as a binary classification problem. The project compares multiple machine learning models—including Logistic Regression, Decision Tree, and Random Forest—and includes steps for data cleaning, feature engineering, and model evaluation.

## Project Structure

## Features
- **Data Cleaning & Feature Engineering:**  
  - Creation of a target variable based on next-day price movement.
  - Calculation of technical indicators such as the 10-day SMA and deviation from SMA.
- **Modeling:**  
  - Baseline model: Logistic Regression.
  - Non-linear model: Decision Tree.
  - Ensemble model: Random Forest.
- **Hyperparameter Tuning:**  
  - Grid Search for optimizing the Decision Tree model.
- **Evaluation:**  
  - Accuracy, precision, recall, F1-score, confusion matrices, and visualizations.

## Dependencies
The project requires the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- yfinance
- scikit-learn

You can install these dependencies using pip:
```bash
pip install -r requirements.txt
```

## How to Run the Project

### Option 1: Local Setup

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/Alisherg/nvda.git
   ```
2. **Change Directory and Install Dependencies:**
    ```bash
    cd nvda
    pip install -r requirements.txt
    ```
3. **Run the Notebook:**
    ```bash
    jupyter notebook supervised_learning_nvda.ipynb
    ```

### Option 2: Google Colab

1. **Upload Notebook to Google Colab:**
   - Open Google Colab.
   - Click on `File > Upload Notebook` and select `NVDA_Stock_Prediction.ipynb` from your local machine.

2. **Run the Notebook on Colab:**
   - Once uploaded, run each cell in sequence.
   - Google Colab comes pre-installed with most required libraries, but if any are missing, add a cell with:

3. **Clear All Outputs Before Running (Optional):**
   - To start with a clean notebook, click on `Edit > Clear all outputs` before running the cells.

### Additional Notes

- **Data:** The project uses historical stock data from Yahoo! Finance via the `yfinance` library. No manual download is required.
- **Results:** The notebook includes detailed visualizations and performance metrics. Make sure to run all cells to reproduce the analysis.
- **Contributions:** Feel free to fork the repository and submit pull requests if you have improvements or new ideas.
