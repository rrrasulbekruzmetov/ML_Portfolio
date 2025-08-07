# Air-Quality-Index-Prediction
A Machine Learning(ML) project to predict Air Quality Index (AQI) based on pollutant levels using regression models and real-world air pollution data.

# What is AQI?

The **Air Quality Index** (AQI) is a standardized indicator for reporting air quality.  
It is calculated based on the concentrations of major air pollutants such as PM2.5, PM10, NO₂, SO₂, CO, and O₃. AQI values help determine the level of health concern for the general public.

Below is the AQI categorization:

| AQI Level                     | AQI Range |
|------------------------------|------------|
| Good                         | 0 – 50     |
| Moderate                     | 51 – 100   |
| Unhealthy                    | 101 – 150  |
| Unhealthy for Strong People  | 151 – 200  |
| Hazardous                    | 201+       |

### Project Goal

The goal of this project is to develop a **regression model** that can accurately predict AQI values based on pollutant readings.  
This helps in:
 - Early warnings for public health
 - Environmental monitoring
 - Governmental and industrial planning

### Approach

We preprocess the dataset, perform exploratory analysis, and train a **Random Forest Regressor**. The model's performance is evaluated using common regression metrics, and predictions are visualized for validation.

---

### Code & Workflow

The main code resides in the Jupyter notebook (`Air_Quality_Index.ipynb`) and follows these steps:

1. **Data Loading & Cleaning**  
   - Import the `AirQualityUCI.csv` dataset.  
   - Handle missing values and filter relevant pollutant columns.

2. **Exploratory Data Analysis (EDA)**  
   - Visualize distributions of pollutants and AQI.  
   - Analyze correlations between features and the target AQI.

3. **Feature Selection & Engineering**  
   - Select key pollutant variables as input features.  
   - Optionally, engineer additional features if needed.

4. **Model Training**  
   - Split data into training and testing sets.  
   - Train a Random Forest Regression model on the training data.

5. **Model Evaluation**  
   - Evaluate predictions using metrics such as:  
     - **Root Mean Squared Error (RMSE)**  
     - **Mean Absolute Error (MAE)**  
     - **R² Score (Coefficient of Determination)**  
   - Plot actual vs. predicted AQI values to visually assess performance.

6. **Results Interpretation**  
   - The R² score indicates how well the model explains variance in AQI.  
   - Lower RMSE and MAE values indicate better prediction accuracy.

This structured workflow enables reproducible and transparent AQI prediction, serving as a foundation for further enhancements or deployment.
