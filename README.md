# Air Quality Index (AQI) Prediction Using KNN Regression

## Project Overview

This project builds a machine learning regression model to predict the Air Quality Index (AQI) based on environmental pollutant data from various Indian cities. Using K-Nearest Neighbors (KNN) regression, the model learns from pollutant concentration features to estimate AQI values, helping understand pollution levels and assist environmental monitoring efforts.

---

## Dataset

- **Source:** [Air Quality Data in India - Kaggle](https://www.kaggle.com/datasets/rohanrao/air-quality-data-in-india)
- **Description:** The dataset contains daily air quality measurements from multiple Indian cities, including concentrations of various pollutants (PM2.5, PM10, NO, NO2, CO, SO2, O3, Benzene, etc.) and the corresponding AQI.

---

## Features Used

- PM2.5  
- PM10  
- NO  
- NO2  
- NOx  
- CO  
- SO2  
- O3  
- NH3  
- Benzene  
- Toluene  
- Xylene  

---

## Project Steps

1. **Data Loading & Cleaning**  
   - Uploaded dataset in Google Colab.  
   - Checked and handled missing values by dropping rows missing AQI and imputing other numeric columns with column means.

2. **Feature Selection**  
   - Selected pollutant concentration columns as features.  
   - Target variable: AQI.

3. **Data Preprocessing**  
   - Train-test split (80%-20%).  
   - Scaled features using StandardScaler since KNN depends on distance measures.

4. **Model Training**  
   - Trained KNN regression with 5 neighbors on the training data.

5. **Model Evaluation**  
   - Evaluated with R² score and Mean Squared Error on train and test sets.  
   - Visualized results using residual plots and actual vs predicted AQI scatter plots.

6. **Visualization**  
   - Boxplot of AQI distribution across Indian cities to understand pollution variation.

---

## How to Run

1. Upload the `city_day.csv` dataset when prompted in Google Colab.  
2. Run all cells sequentially.  
3. View model performance metrics and visualizations generated at the end.

---

## Results Summary

- The KNN regression model predicts AQI values based on pollutant data with reasonable accuracy.  
- Visualizations reveal pollution spread across cities and highlight model prediction errors.  
- Residual distribution shows if the model errors are randomly distributed or biased.

---

## Future Improvements

- Hyperparameter tuning (e.g., varying number of neighbors).  
- Try other regression models like Random Forest, Gradient Boosting.  
- Include additional features like weather data, temporal trends.  
- Implement cross-validation for robust evaluation.  
- Geospatial visualization of AQI levels.

---

## Dependencies

- Python 3.x  
- pandas  
- numpy  
- matplotlib  
- seaborn  
- scikit-learn  
- Google Colab environment (for easy dataset upload and execution)

---

## Contact

For questions or suggestions, feel free to reach out.

