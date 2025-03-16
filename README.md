# Flight Price Data Preprocessing & Feature Engineering  

## 📌 Project Overview  
This project focuses on **cleaning and transforming flight price data** to prepare it for machine learning models. The dataset initially contained several categorical and date-time variables, which were converted into a structured numerical format using **feature engineering techniques** like date-time extraction and one-hot encoding.  

## 📊 Dataset Details  
### 🔹 Columns Before Feature Engineering:  
- `Airline`, `Date_of_Journey`, `Source`, `Destination`, `Route`,  
  `Dep_Time`, `Arrival_Time`, `Duration`, `Total_Stops`,  
  `Additional_Info`, `Price`  

### 🔹 Columns After Feature Engineering:  
- `Total_Stops`, `Price`, `Date`, `Month`, `Year`, `Arrival_Hour`,  
  `Arrival_Minute`, `Dep_Hour`, `Dep_Minute`, `Duration_Hour`, `Duration_Minute`  
- **One-hot encoded categorical variables** for `Airline`, `Source`, and `Destination`  

## ⚙️ Feature Engineering Steps  
✅ **Extracted date-time components:**  
- Created `Date`, `Month`, and `Year` from `Date_of_Journey`  
- Extracted `Arrival_Hour` and `Arrival_Minute` from `Arrival_Time`  
- Extracted `Dep_Hour` and `Dep_Minute` from `Dep_Time`  
- Converted `Duration` into `Duration_Hour` and `Duration_Minute`  

✅ **Encoded categorical features using One-Hot Encoding:**  
- Transformed `Airline`, `Source`, and `Destination` into multiple binary columns  

✅ **Ensured all features were numerical** to improve model performance  

## 💡 Why Feature Engineering?  
Feature engineering is crucial for **improving model accuracy** and making raw data more meaningful. By converting categorical and date-time values into numerical representations, we enable models to learn better patterns and make accurate predictions.  

## 🛠️ Technologies Used  
- **Python** (Pandas, NumPy, Scikit-learn)  
- **Jupyter Notebook**  
