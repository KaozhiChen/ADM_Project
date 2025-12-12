# ADM Demand Forecasting Project

A demand forecasting project using XGBoost models, based on the M5 Forecasting competition dataset.

## Project Structure

```
ADM_Project/
├── Data/
│   ├── data_preprocessing.ipynb      # Data preprocessing pipeline
│   ├── EDA.ipynb                     # Exploratory data analysis
│   ├── training_data.csv.zip         # Compressed preprocessed training data
│   └── Row_Data/
│       ├── calendar.csv              # Calendar information
│       └── sales_train_evaluation.csv.zip # Compressed raw sales data 
├── images/                           # Visualization outputs
│   ├── fig_corr.png
│   ├── fig_forecast.png
│   ├── fig_importance_*.png
│   └── ...
└── XGBoost.ipynb                     # Main model training and evaluation
```

## Data Note

Due to the large size of the original M5 dataset files, both the raw data and preprocessed training data have been compressed and uploaded:

- **Preprocessed training data**: `Data/training_data.csv.zip`
- **Raw sales data**: `Data/Row_Data/sales_train_evaluation.csv.zip`

To use the project, first extract the compressed files:
```bash
unzip Data/training_data.csv.zip -d Data/
unzip Data/Row_Data/sales_train_evaluation.csv.zip -d Data/Row_Data/
```

## Usage

1. Extract the compressed data files (see Data Note above)
2. Run `XGBoost.ipynb` to train and evaluate the models
3. For data preprocessing, run `Data/data_preprocessing.ipynb` (requires extracted raw data files)

