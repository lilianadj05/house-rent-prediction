# 🏠 House Rent Prediction

## 📌 Project Overview
This project aims to predict fair and unbiased house rent prices based on property characteristics using a machine learning model. By analyzing a dataset of Indian rental properties, the project seeks to identify the key factors that influence rent prices. This information can be beneficial for both landlords and tenants, helping landlords set appropriate prices and tenants find reasonably priced properties.

## 📊 Dataset
The **House Rent Dataset**, sourced from a real estate website in India, contains information on various properties for rent. The dataset includes details such as the number of bedrooms, hall, and kitchen (BHK), property size, floor, and location, as well as the rental price.

## 🔍 Key Findings
1. The most common type of rental property is semi-furnished.
2. Mumbai has the highest average rent, while Kolkata has the lowest.
3. The most influential factors affecting rent prices are Point of Contact, number of bathrooms, and BHK.
4. Size and rent have a moderate positive correlation.

## 📈 Steps
1. **Data Cleaning**: No missing or duplicate values were found, so no data cleaning was required. The **Rent** and **Size** variables were found to be skewed and have outliers, which were addressed in the preprocessing step.
2. **Preprocessing**: To prepare the data for modeling, the skewed Rent and Size columns were transformed using **log and square root transformations**, respectively. Categorical features were converted into numerical representations using **Label Encoding** and **Ordinal Encoding**. The Floor column was also cleaned and converted into a numerical format. Finally, the numerical features were scaled using a **RobustScaler** to handle outliers.
3. **Modeling and Evaluation**: A **Random Forest Regressor** was chosen as the proposed model due to its ability to handle non-linear patterns and its resilience to outliers. A **Linear Regression** model was used as a baseline for comparison. The models were evaluated using R-squared (R^2), Root Mean Squared Error (RMSE), and Mean Absolute Error (MAE). **The Random Forest model, especially after fine-tuning, outperformed the Linear Regression model on all metrics.**

## 💡 Conclusion
The Random Forest Regressor proved to be an effective model for predicting house rent prices, demonstrating higher accuracy and better performance compared to the baseline Linear Regression model. The model successfully identified key features that influence rent, providing valuable insights for both property owners and renters.

## 🔮 Possible Future Works
1. **Explore additional features**: Incorporate other potential factors, such as property age, amenities, and proximity to public transport or key services, which may further improve the model's predictive power.
2. **Implement different machine learning models**: Test other advanced regression algorithms, such as Gradient Boosting or XGBoost, to see if they can achieve even higher accuracy.
3. **Automate the prediction process**: Create a user-friendly interface or API that allows users to input property details and get an instant rent prediction.

## 🤝 Contributors
1. Aquila Kyne Sudiro
2. Caroline Ang
3. Laurel Evelina Widjaja
4. Liliana Djaja Witama
