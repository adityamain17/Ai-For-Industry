🔧 Predictive Maintenance of Industrial Machines (AI4I 2020)
📌 Overview

This project focuses on predicting machine failures using the AI4I 2020 Predictive Maintenance dataset. It combines mechanical engineering concepts with machine learning to analyze operational parameters and identify failure patterns in industrial equipment.

🎯 Objective

To build a classification model that predicts whether a machine will fail based on real-time operating conditions, enabling preventive maintenance and reduced downtime.

⚙️ Mechanical Engineering Context

This project directly relates to core mechanical engineering areas:

Condition monitoring of machinery
Failure analysis (TWF, HDF, PWF, OSF, RNF)
Thermal and mechanical parameter analysis
Power estimation using torque and rotational speed
Reliability engineering & maintenance optimization
📊 Dataset Details

The dataset includes the following parameters:

Air Temperature
Process Temperature
Rotational Speed
Torque
Tool Wear
Machine Type (L, M, H)
Failure Types:
TWF (Tool Wear Failure)
HDF (Heat Dissipation Failure)
PWF (Power Failure)
OSF (Overstrain Failure)
RNF (Random Failure)
🔄 Data Preprocessing
Removed irrelevant columns (UDI, Product ID)
Renamed columns for clarity
Converted categorical data (Type → numeric encoding)
Combined multiple failure types into a single Machine Failure label
Created a new feature:
Power = Torque × Rotational Speed
Handled imbalanced data observation
Outlier treatment using IQR method
Feature scaling using:
StandardScaler
Normalizer
🧠 Models Implemented

The following machine learning models were trained and evaluated:

Naive Bayes (GaussianNB)
Decision Tree Classifier
Random Forest Classifier
Random Forest (with multiple trees)
Logistic Regression
📈 Model Evaluation

Models were evaluated using:

Accuracy
Precision
Recall
Confusion Matrix
ROC Curve
🔍 Key Insights
Machine failure depends strongly on torque, rotational speed, and temperature conditions
Combining failure types simplifies prediction without major loss of information
Feature engineering (Power) improves understanding of machine behavior
Ensemble methods (Random Forest) perform better for this type of problem
🛠️ Tools & Libraries
Python
Pandas, NumPy
Matplotlib, Seaborn
Scikit-learn
Jupyter Notebook
📂 Project Structure
├── AI4I101.ipynb        # Main implementation notebook
├── dataset.csv          # AI4I dataset (external)
├── README.md            # Documentation
🚀 Applications
Predictive maintenance in manufacturing plants
Monitoring rotating machinery
Industrial automation systems
Smart factories (Industry 4.0)
📜 Conclusion

This project demonstrates how mechanical system parameters can be integrated with machine learning to predict failures effectively, reducing downtime and improving system reliability.
