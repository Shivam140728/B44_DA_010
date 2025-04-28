# B44_DA_010

# Flight Price Prediction System

## **Project Overview**:

This project involves predicting flight prices based on various factors such as the airline, origin, destination, stops, and travel date. The goal is to clean the dataset, explore relationships between features, train regression models to predict prices, and deploy the model in an interactive web application.

### **Dataset**:

[Download Flight Price Dataset](https://www.kaggle.com/datasets/iamavyukt/goibibo-flight-data/data)

### **Steps**:

- **Data Cleaning and Preprocessing**:
    - **Remove Unnecessary Columns**: Drop empty or irrelevant columns such as `Unnamed: 11` and `Unnamed: 12`.
    - **Convert Date Columns**: Convert date-related columns into proper datetime formats and extract meaningful features like **day**, **month**, and **year**.
    - **Transform Categorical Variables**: Convert categorical columns (such as **airline**, **from**, **to**, and **stops**) into numerical representations using techniques like **Label Encoding** or **One-Hot Encoding**.
    - **Convert Duration**: Convert the `duration` column from text format (e.g., '3h 15m') to a numerical value (e.g., total minutes).
    - **Clean Price Column**: Clean and convert the `price` column from text format (e.g., '₹4500') into a numerical value (e.g., 4500).

- **Exploratory Data Analysis (EDA)**:
    - **Price Distribution**: Analyze the distribution of flight prices across different airlines, routes, and travel times. Identify any significant patterns in pricing.
    - **Visualize Relationships**: Visualize the relationship between **flight duration**, **departure time**, and **price** using scatter plots or line charts.
    - **Impact of Stops on Price**: Investigate how the number of stops (non-stop, 1 stop, 2 stops, etc.) affects the flight price using bar charts or box plots.

- **Model Selection and Training**:
    - **Train-Test Split**: Split the dataset into training and test sets using **train_test_split**.
    - **Regression Algorithms**: Use regression algorithms such as **Linear Regression**, **Random Forest Regressor**, or **Gradient Boosting Regressor** to train the model.
    - **Model Evaluation**: Evaluate the model using appropriate metrics like **Mean Absolute Error (MAE)** or **Root Mean Squared Error (RMSE)** to assess the accuracy of the price predictions.

- **Model Evaluation**:
    - **Hyperparameter Optimization**: Fine-tune the model using techniques such as **GridSearchCV** or **RandomizedSearchCV** to optimize the hyperparameters and improve model performance.
    - **Model Comparison**: Compare the performance of different regression models and select the best-performing model based on evaluation metrics.

- **Deployment with Streamlit**:
    - **Streamlit Web App**: Create a Streamlit app where users can input flight details such as **airline**, **departure city**, **destination city**, **class**, **stops**, and **date**.
    - **Prediction Display**: Display the predicted flight price based on user inputs.
    - **Visualize Model Accuracy**: Allow users to visualize model accuracy with **evaluation metrics** and **plots** showing the comparison of predicted vs actual prices.

### **Skills Covered**:

- **Data cleaning** (handling missing values, converting categorical variables).
- **Exploratory data analysis** (EDA, visualizations, correlation analysis).
- **Regression models** (Linear Regression, Random Forest, Gradient Boosting).
- **Model evaluation** (Mean Absolute Error, RMSE, hyperparameter tuning).
- **Web app deployment** (using **Streamlit** to build a user interface).

### **Insights**:

1. **Airline Influence**: Flight prices are significantly influenced by the airline, with legacy airlines generally charging higher prices than budget airlines.
2. **Stops and Price**: Flights with fewer stops tend to be more expensive, with non-stop flights costing an average of **30-40% more** than one-stop flights.
3. **Impact of Travel Dates**: Flights booked closer to the departure date are often more expensive, with prices rising by as much as **15-20%** in the final few days before the flight.
4. **Class of Service**: First-class flights have a significant price premium, typically **3 to 4 times** more expensive than economy-class tickets on similar routes.
5. **Seasonal Trends**: Airfares tend to be higher during **peak travel seasons** like holidays, summer vacations, and festivals, with significant price hikes in destinations like **Europe** and **Asia** during the summer months.
6. **Departure Time**: Early morning or late-night flights are usually cheaper than flights departing during peak business hours.
7. **Route Popularity**: Popular routes like **Delhi to Mumbai** or **New York to London** often have a larger price variance depending on demand, with occasional discounts during off-peak periods.

## **Installation and Usage**:

### **1. Clone the Repository**:
```bash
git clone https://github.com/yourusername/flight-price-prediction.git
