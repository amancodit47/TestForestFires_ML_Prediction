# Forest Fire Algerian ML Project

## Table of Contents
- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Problem Statement](#problem-statement)
- [Approach](#approach)
- [Technologies Used](#technologies-used)
- [Model Performance](#model-performance)
- [How to Use](#how-to-use)
- [Examples](#examples)
- [Future Enhancements](#future-enhancements)
- [Acknowledgements](#acknowledgements)

---

![image alt](https://github.com/Ktrimalrao/Forest_fire_Algerian_ML-project/blob/2bc9e79e0b33cba223ef8b806dd5c0d764099346/Screenshot%202024-12-29%20122115.png)

## Project Overview
The **Forest Fire Algerian ML Project** aims to predict the likelihood and severity of forest fires in Algeria based on weather conditions and other environmental factors. The model developed can help authorities and environmental agencies take preventive measures to minimize fire risks.

---

## Dataset Description
The dataset consists of 244 instances, which include data from two regions in Algeria:

- **Bejaia Region**: Located in the northeast of Algeria.
- **Sidi Bel-abbes Region**: Located in the northwest of Algeria.

### Dataset Characteristics

- **Time Period**: The data spans from **June 2012 to September 2012**.
- **Instances**: 
  - **122 instances** for each region. 
  - **Fire cases**: 138 instances.
  - **No fire cases**: 106 instances.
- **Attributes**: The dataset has **11 attributes** and **1 target attribute** (class).

### Attribute Information

1. **Date**: Observation date in the format `DD/MM/YYYY`.  
   Includes:
   - Day
   - Month (`June` to `September`)
   - Year (2012)

2. **Temperature (Temp)**:  
   - The maximum temperature at noon, measured in degrees Celsius.  
   - Range: 22 to 42.

3. **Relative Humidity (RH)**:  
   - The relative humidity percentage.  
   - Range: 21% to 90%.

4. **Wind Speed (Ws)**:  
   - Wind speed measured in km/h.  
   - Range: 6 to 29.

5. **Rain**:  
   - Total rainfall in a day, measured in mm.  
   - Range: 0 to 16.8.

6. **Fine Fuel Moisture Code (FFMC)**:  
   - An index from the FWI system that represents moisture content in fine fuels.  
   - Range: 28.6 to 92.5.

7. **Duff Moisture Code (DMC)**:  
   - Represents the moisture content in the duff layer.  
   - Range: 1.1 to 65.9.

8. **Drought Code (DC)**:  
   - Represents the moisture content in the deep organic layers.  
   - Range: 7 to 220.4.

9. **Initial Spread Index (ISI)**:  
   - Indicates the initial rate of fire spread.  
   - Range: 0 to 18.5.

10. **Buildup Index (BUI)**:  
    - Represents the total amount of fuel available for combustion.  
    - Range: 1.1 to 68.

11. **Fire Weather Index (FWI)**:  
    - A comprehensive index representing fire risk.  
    - Range: 0 to 31.1.

12. **Classes**:  
    - The target attribute with two possible values:  
      - **Fire**
      - **No Fire**

---

## Problem Statement
Predict whether a forest fire will occur and classify its severity based on meteorological and environmental data. The project focuses on using machine learning models to identify patterns and relationships within the dataset.

---

## Approach
1. **Data Preprocessing**
   - Handling missing values.
   - Feature scaling and encoding.
   - Splitting data into training and testing sets.

2. **Exploratory Data Analysis (EDA)**
   - Visualizing key features and their relationships.
   - Identifying correlations and trends.

3. **Model Development**
   - Algorithms used: Logistic Regression, Random Forest, Decision Tree, Gradient Boosting.
   - Hyperparameter tuning for optimal performance.

4. **Evaluation**
   - Metrics: Accuracy, Precision, Recall, F1-score.
   - Confusion Matrix and ROC curve analysis.

---

## Technologies Used
- **Programming Language**: Python
- **Libraries**: 
  - pandas, numpy
  - scikit-learn
  - matplotlib, seaborn
  - Flask (for deployment)

---

## Model Performance
The best-performing model is **Ridge Regression model**, achieving the following metrics:
- **R2 Score**: 98.42%
- **Mean absolute error**: 0.56
  
---

## How to Use

1. **Clone the Repository**
   ```bash
   git clone https://github.com/Ktrimalrao/Forest_fire_Algerian_ML-project.git
   ```

2. **Install Dependencies**
   ```bash
   pip install -r requirements.txt
   ```

3. **Run the Project**
   ```bash
   python app.py
   ```

4. **Access the Application**
   Open your browser and navigate to `http://127.0.0.1:5000`.

---

## Examples

### Input:
- Temperature: 30°C
- Relative Humidity: 40%
- Wind Speed: 15 km/h
- Rainfall: 0 mm

### Output:
- Fire Severity: **High Risk**

---

## Future Enhancements
- Integration with real-time weather APIs for dynamic predictions.
- Expand the dataset to include more regions.
- Develop a mobile application for accessibility.

---

## Acknowledgements
We thank the creators of the Algerian forest fire dataset for their valuable contribution to environmental and disaster management research.

**Author**: Ktrimalrao  
**GitHub**: [https://github.com/Ktrimalrao](https://github.com/Ktrimalrao)
**LinkdIn**: [LinkdIN](https://www.linkedin.com/in/k-trimal-rao-397924253/)
