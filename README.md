# COVID-19 Deaths Prediction

## Project Overview
This project is part of an academic assignment focused on applying machine learning techniques to predict real-world societal threats. The chosen topic is **COVID-19 deaths prediction**, where I developed a machine learning model to forecast new cases based on historical data.  

The project involves:
- **Data Visualisation:** Analysing trends in COVID-19 deaths.
- **Data Preprocessing:** Cleaning, transforming, and preparing data for modelling.
- **Model Development:** Implementating a machine learning model for case prediction.
- **Model Optimisation:** Fine-tuning parameters for improved accuracy.
- **Performance Analysis:** Evaluating results using performance metrics, graphical analysis, and Explainable AI (XAI) techniques.

## Dataset
The dataset used for this project is the [OWID COVID-19 dataset](https://raw.githubusercontent.com/owid/covid-19-data/refs/heads/master/public/data/owid-covid-data.csv), which contains various COVID-19 related statistics for multiple countries. The dataset is accessed directly from the OWID GitHub repository.
 
## Data Preprocessing

The following steps were performed to clean and preprocess the data:
- Filtered data for the United Kingdom only.
- Converted the `date` column to the datetime format.
- Select revelant columns including case numbers and deaths.
- Removed NaN values.
- Filtered data from 2nd February 2020 to 22nd October 2023.
- Removed rows where `new_deaths` was zero.
- Normalised the target variable (`new_deaths`) using MinMaxScaler.
- Created sequences of 30-day windows for LSTM model input.

## Model Architecture

A deep learning model using LSTM was implemented with the following architecture:
- **Input Layer:** Sequence of 30 previous days.
- **Two LSTM Layers:** 50 units each.
- **Dense Output Layer:** Predicts the number of new deaths.
- **Optimiser:** Adam.
- **Loss Function:** Mean Squared Error (MSE).
- **Early Stopping:** To prevent overfitting.

## Model Training

The dataset was split into training (80%) and validation (20%) sets. The model was trained for 50 epochs with a batch size of 32, using early stopping to optimise performance.

## Model Evaluation

The model's performance was evaluated using:
- **Mean Absolute Error (MAE)**
- **Mean Squared Error (MSE)**
- **Root Mean Squared Error (RMSE)**
- **$R^2$ Score**

A plot of training vs validation loss was generated to assess model convergence.

## Results

After training, the model made predictions on the validation set. The results were compared to actual values using evaluation metrics.

## Dependencies

To run this project, install the required Python packages:

```pip install pandas numpy scikit-learn tensorflow matplotlib```

## Running the Code

To execute the code, simply run the script in a Python environment:

```python covid_deaths_prediction.ipynb```

## Author:
- [Riya Chandaria](https://github.com/riyachandaria)

