# AI-ML Assignment – 6

# Weather Condition Classification using Support Vector Machine (SVM) and Open-Meteo API

## Student Details

| Field | Details |
|-------|---------|
| **Name** | Rohan Ramdhan Decharwal |
| **Batch** | AI/ML Internship – Batch 1(A) |
| **Mentor** | Nishant Shrivastava |
| **University** | VIT Bhopal University |
| **Course** | B.Tech Computer Science and Engineering (AI & ML) |

---

## Objective

The objective of this assignment is to develop a **Support Vector Machine (SVM)** classifier to classify weather conditions as **Warm** or **Cool** using meteorological data obtained from the **Open-Meteo API**. The model is trained using weather parameters such as temperature, relative humidity, surface pressure, and wind speed after performing data preprocessing and feature scaling.

---

## API Documentation Link

- https://open-meteo.com/
- Archive API: https://archive-api.open-meteo.com/

---

## Libraries Used

- Python
- Pandas
- NumPy
- Requests
- Scikit-learn
- Matplotlib

---

## Methodology

1. Collected historical weather data using the **Open-Meteo Archive API**.
2. Converted the JSON response into a Pandas DataFrame.
3. Created a new target column **Weather_Class**:
   - **Warm** → Temperature ≥ 25°C
   - **Cool** → Temperature < 25°C
4. Checked for missing values.
5. Selected the required input features.
6. Encoded the target variable using **LabelEncoder**.
7. Split the dataset into **80% training** and **20% testing** sets.
8. Standardized the feature values using **StandardScaler**.
9. Trained a **Support Vector Machine (SVM)** classifier with the **RBF kernel**.
10. Evaluated the model using:
    - Accuracy
    - Precision
    - Recall
    - F1-Score
    - Confusion Matrix

---

## Input Features

- Temperature
- Relative Humidity
- Surface Pressure
- Wind Speed

## Target Variable

**Weather_Class**

- Warm → Temperature ≥ 25°C
- Cool → Temperature < 25°C

---

## Results

The Support Vector Machine (SVM) model successfully classified weather conditions into **Warm** and **Cool** categories. The model was evaluated using Accuracy, Precision, Recall, F1-Score, and a Confusion Matrix. Feature scaling improved the model's performance, and the RBF kernel effectively captured the non-linear relationships between weather parameters. The results indicate that the model performs well for weather classification based on historical meteorological data.

---

## Conclusion

This project demonstrates the application of the Support Vector Machine (SVM) algorithm for weather condition classification using historical data obtained from the Open-Meteo API. Features such as temperature, humidity, surface pressure, and wind speed were used to train the model after appropriate preprocessing and feature scaling. The SVM classifier effectively separated the weather classes and achieved reliable classification performance. Feature scaling proved to be essential because SVM relies on distance-based optimization. While SVM provides high accuracy and performs well on complex datasets, one limitation is that its performance may decrease when the dataset is highly imbalanced or very large. Overall, SVM is a powerful and effective algorithm for weather classification tasks.

---

## Repository Structure

```
Assignment-6/
│── Assignment_6.ipynb
│── README.md
```

---

## Author

**Rohan Ramdhan Decharwal**

**AI/ML Internship – Batch 1(A)**

**Mentor:** Nishant Shrivastava
