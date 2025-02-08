# COVID-19 Case Prediction

## Project Overview
This project is part of an academic assignment focused on applying machine learning techniques to predict real-world societal threats. The chosen topic is **COVID-19 case prediction**, where I developed a machine learning model to forecast new cases based on historical data.  

The project involves:
- **Data Visualisation:** Analysing trends in COVID-19 cases.
- **Data Preprocessing:** Cleaning, transforming, and preparing data for modelling.
- **Model Development:** Implementating a machine learning model for case prediction.
- **Model Optimisation:** Fine-tuning parameters for improved accuracy.
- **Performance Analysis:** Evaluating results using performance metrics, graphical analysis, and Explainable AI (XAI) techniques.

## Dataset
- **Source:** [OWID COVID-19 Data](https://raw.githubusercontent.com/owid/covid-19-data/refs/heads/master/public/data/owid-covid-data.csv)
- **Features Used:**
  - `date`: Date of recorded data
  - `new_cases`: Daily new COVID-19 cases
  - Additional relevant features may be considered
 
## Methodology
1. **Data Preprocessing**
    - Handling missing values
    - Feature engineering
    - Data normalisation
2. **Exploratory Data Analysis (EDA)**
    - Trend and seasonality analysis
    - Data visualisation
3. **Model Selection & Training**
    - **Machine Learning Model:** ARIMA, LSTM, or an AutoML approach
    - **Hyperparameter Optimisation:** Improving model performance
4. **Evaluation Metrics:**
    - RMSE (Root Mean Squared Error)
    - MAE (Mean Absolute Error)
    - XAI techniques for interpretability

## Tools & Technologies
- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn, TensorFlow/Pytorch
- **Development Platforms:** GitHub, Google Colab
- **AutoML:** Tools like AutoKeras, H2O.ai

## Repository Structure:
📂 covid19-prediction  
│-- 📂 data/                # Raw and processed data  
│-- 📂 notebooks/           # Jupyter notebooks for EDA and modelling  
│-- 📂 models/              # Trained model files  
│-- preprocess_data.py      # Data cleaning and preparation script  
│-- train_model.py          # Model training script  
│-- predict.py              # Prediction script  
│-- README.md               # Project documentation  
│-- requirements.txt        # Required dependencies  

## Contributors:
- [Riya Chandaria](https://github.com/riyachandaria)

