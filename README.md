# XAI and Anomaly Detection in Financial Data

## 📊 Project Overview

This project implements **Explainable AI (XAI)** techniques for **anomaly detection** in financial data, specifically focusing on NIFTY 50 stock market data. The project combines machine learning algorithms with interpretability frameworks to identify unusual patterns in stock price movements while providing clear explanations for the detected anomalies.

## 🎯 Objectives

- **Anomaly Detection**: Identify unusual patterns and outliers in stock price movements
- **Explainable AI**: Provide interpretable explanations for detected anomalies using SHAP and LIME
- **Financial Analysis**: Analyze technical indicators and market patterns
- **Risk Assessment**: Help identify potential market risks and opportunities

## 🗂️ Project Structure

```
XAI-and-Anomaly-Detection-in-Financial-Data/
│
├── data/
│   ├── raw/                          # Original NIFTY 50 stock CSV files
│   │   ├── ADANIPORTS.csv
│   │   ├── RELIANCE.csv
│   │   ├── TCS.csv
│   │   └── ... (50 companies total)
│   │
│   ├── processed/                    # Cleaned and processed datasets
│   │   ├── nifty50_cleaned.csv      # Merged and cleaned data
│   │   ├── nifty50_with_anomalies.csv # Data with anomaly labels
│   │   └── preprocessed_with_indicators.csv # Technical indicators
│   │
│   └── others/                       # Additional metadata
│       ├── NIFTY50_all.csv
│       └── stock_metadata.csv
│
├── notebooks/
│   ├── preprocessing.ipynb          # Data cleaning and preparation
│   └── implementation.ipynb         # Anomaly detection and XAI
│
├── requirements.txt                 # Python dependencies
└── README.md                       # Project documentation
```

## 🛠️ Technologies Used

- **Python 3.x**
- **Data Processing**: Pandas, NumPy
- **Machine Learning**: Scikit-learn, TensorFlow
- **Visualization**: Matplotlib, Seaborn
- **Explainable AI**: SHAP, LIME
- **Technical Analysis**: Custom indicators (RSI, Bollinger Bands, SMA, EMA, OBV)

## 📋 Features

### Data Processing
- **Multi-company Data Integration**: Merges data from 50 NIFTY companies
- **Time Series Filtering**: Focuses on post-2016 data for relevance
- **Data Cleaning**: Handles missing values and data inconsistencies

### Technical Indicators
- **Simple Moving Average (SMA)** - 20-day period
- **Exponential Moving Average (EMA)** - 20-day period
- **Relative Strength Index (RSI)** - 14-day period
- **Bollinger Bands** - 20-day with 2 standard deviations
- **On-Balance Volume (OBV)** - Volume trend analysis
- **Volume Moving Average (VMA)** - 20-day period

### Anomaly Detection
- Machine learning models to identify unusual market patterns
- Statistical methods for outlier detection
- Time series anomaly identification

### Explainable AI
- **SHAP (SHapley Additive exPlanations)**: Model-agnostic explanations
- **LIME (Local Interpretable Model-agnostic Explanations)**: Local feature importance
- Feature importance analysis for anomaly detection

## 🚀 Getting Started

### Prerequisites

- Python 3.7 or higher
- Jupyter Notebook or JupyterLab

### Installation

1. **Clone the repository**:
   ```bash
   git clone <repository-url>
   cd XAI-and-Anomaly-Detection-in-Financial-Data
   ```

2. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

3. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

### Usage

1. **Data Preprocessing**:
   - Open `notebooks/preprocessing.ipynb`
   - Run all cells to clean and prepare the data
   - This will generate processed datasets in `data/processed/`

2. **Anomaly Detection & XAI**:
   - Open `notebooks/implementation.ipynb`
   - Run cells to calculate technical indicators
   - Execute anomaly detection algorithms
   - Generate XAI explanations

## 📈 Data Sources

The project uses **NIFTY 50** stock data including:

- **50 Major Indian Companies**: ADANIPORTS, ASIANPAINT, AXISBANK, BAJAJ-AUTO, BHARTIARTL, RELIANCE, TCS, INFOSYS, and more
- **Time Period**: 2016 onwards
- **Data Fields**: Date, Open, High, Low, Close, Volume
- **Frequency**: Daily stock prices

## 🔬 Methodology

### 1. Data Preprocessing
- Merge individual company CSV files
- Filter data from 2016 onwards
- Handle missing values and outliers
- Normalize data for analysis

### 2. Feature Engineering
- Calculate technical indicators
- Create lag features
- Generate rolling statistics
- Compute price movements and volatility

### 3. Anomaly Detection
- Statistical methods (Z-score, IQR)
- Machine learning approaches (Isolation Forest, One-Class SVM)
- Time series anomaly detection
- Ensemble methods for robust detection

### 4. Explainable AI
- SHAP values for global and local explanations
- LIME for individual prediction explanations
- Feature importance ranking
- Visualization of decision boundaries

## 📊 Results & Insights

The project provides:

- **Anomaly Identification**: Detected unusual market patterns and events
- **Feature Importance**: Understanding which indicators contribute most to anomalies
- **Interpretable Models**: Clear explanations for each detected anomaly



## 📄 License

This project is open source and available under the [MIT License](LICENSE).


---

**Note**: This project is for educational and research purposes.