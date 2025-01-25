# Predictive Maintenance Dashboard

Welcome to the **Predictive Maintenance Dashboard**! This interactive application leverages machine learning to provide actionable insights for industrial machinery monitoring and maintenance. Designed to minimize downtime and optimize operations, the dashboard integrates data visualization, real-time predictions, and anomaly detection into an intuitive interface.

---

## **Features**

### 1. **Predictive Models**
- **Remaining Useful Life (RUL) Prediction**:
  - Using a **RandomForestRegressor**, the system predicts how many hours of operation remain before maintenance is required.
- **Maintenance Classification**:
  - A **RandomForestClassifier** determines whether a machine needs maintenance (`Needs Maintenance`) or is functioning normally (`Normal`).

### 2. **Anomaly Detection**
- Implements **K-Means Clustering** to detect anomalies in sensor readings.
  - Results indicate whether the readings are within normal operating parameters or if an anomaly has occurred.

### 3. **Interactive Visualizations**
- Explore detailed visualizations of your data, including:
  - **Histograms** for sensor readings.
  - **Scatter plots** comparing operational hours to sensor outputs.
  - **Line charts** illustrating Remaining Useful Life trends over time.
- Overlay user-generated input values on visualizations for context.

### 4. **Dynamic User Input**
- Input sensor readings manually or generate random values to simulate real-world data.
- Easily navigate between input, results, and visualizations through the sidebar menu.

### 5. **Real-Time Alerts**
- Visual indicators for:
  - Maintenance needs (`⚠️ Maintenance is required!`).
  - Anomalous sensor readings (`⚠️ Anomaly detected in sensor readings!`).

### 6. **Data Handling**
- Automatically preprocesses data:
  - Handles missing values with forward fill.
  - Normalizes sensor readings using `StandardScaler` for consistent model performance.

---

## **Technology Stack**

The dashboard is built using the following tools and technologies:

- **Streamlit**:
  - For creating the interactive user interface.
- **scikit-learn**:
  - Implements machine learning models for regression, classification, and clustering.
- **Matplotlib & Seaborn**:
  - For creating visualizations to explore and understand the data.
- **NumPy & Pandas**:
  - For efficient data manipulation and preprocessing.

---

## **How to Use the Dashboard**

### **1. Navigate Through the Sidebar Menu**
The sidebar contains the following options:
- **Home**: Learn about the dashboard and its capabilities.
- **Historical Data**: View a preview of the loaded machinery dataset.
- **Input Data**: Input or generate sensor readings and operational hours.
- **Results**: View model predictions for RUL, maintenance status, and anomaly detection.
- **Visualizations**: Explore interactive charts and plots for deeper insights.

### **2. Input Data for Predictions**
- **Manual Input**: Use sliders to enter sensor readings and operational hours.
- **Random Generation**: Automatically generate sensor readings within the dataset range.
- Submit your inputs to receive predictions in the **Results** section.

### **3. View Predictions**
- Access the **Results** section to:
  - See predicted Remaining Useful Life (RUL).
  - Check whether the machine needs maintenance.
  - Identify any anomalies in the data.

### **4. Visualize Your Data**
- Access the **Visualizations** section to:
  - Understand trends and patterns in historical data.
  - Compare input values to dataset distributions and trends.

---

## **Example Use Case**

1. **Historical Data**:
   - Review the past performance of machinery using historical records.
2. **Input Data**:
   - Input real-time sensor readings or generate simulated data.
3. **Results**:
   - Predict Remaining Useful Life (RUL).
   - Get alerts if maintenance is needed or anomalies are detected.
4. **Visualizations**:
   - Analyze trends and identify patterns to optimize operations.

---

## **Setup Instructions**

1. **Prerequisites**:
   - Python 3.7+
   - Required libraries:
     ```bash
     pip install streamlit pandas numpy matplotlib seaborn scikit-learn
     ```
2. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-repo/predictive-maintenance-dashboard.git
   cd predictive-maintenance-dashboard
   ```
3. **Run the Application**:
   ```bash
   streamlit run app.py
   ```
4. **Access the Dashboard**:
   - Open your browser and navigate to the URL provided by Streamlit (e.g., `http://localhost:8501`).

---

## **Future Enhancements**

- **Explainable AI**:
  - Integrate SHAP values to provide deeper insights into model predictions.
- **Real-Time Streaming**:
  - Enable real-time data ingestion from IoT sensors.
- **Dockerization**:
  - Containerize the application for scalable deployment.
- **Alert System Integration**:
  - Add email or SMS notifications for maintenance and anomaly alerts.



## **License**
This project is licensed under the MIT License. See the LICENSE file for more details.

---

Thank you for using the Predictive Maintenance Dashboard! 🚀

