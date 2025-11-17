# Energy Efficiency Analysis with XGBoost and Streamlit

Energy Efficiency Analysis with XGBoost and Streamlit
Overview

This project utilizes the Energy Efficiency dataset from the UCI Machine Learning Repository to analyze how various building characteristics influence overall energy performance.
The original study simulated 12 different building shapes in Ecotect, varying parameters such as surface area and overall height.
The dataset contains 768 samples, 8 input features, and 2 target variables:

Heating Load (Y1)

Cooling Load (Y2)

Dataset link:
https://archive.ics.uci.edu/dataset/242/energy+efficiency

Project Goal

The objective of this project is to build a predictive tool that helps homeowners, architects, and individuals planning residential construction to estimate heating and cooling energy requirements based on house characteristics.

To enhance user experience, the dataset’s features have been renamed, simplified, and consolidated, making the inputs intuitive and easy to understand.
Based on user inputs such as building shape, orientation, glazing area, and other structural factors, the application predicts heating and cooling loads and suggests a suitable HVAC system for optimal energy efficiency.

Approach

Data Exploration
Performed exploratory analysis to understand feature behavior, correlations, and target distributions.

Model Development
Trained two independent XGBoost regression models — one for Heating Load (Y1) and another for Cooling Load (Y2).

Feature Importance Analysis
Identified the most influential features contributing to energy efficiency. Results are visualized through a feature-importance bar chart.

Model Serialization
Saved trained models as .pkl (Pickle) files for efficient reuse in the Streamlit application.

Streamlit Application
Built an interactive and user-friendly web interface that accepts building parameters and outputs real-time predictions for both loads along with recommended HVAC options.

Usage

Ensure the required dependencies are installed before running the application.

Install packages:

pip install -r requirements.txt


Run the Streamlit app:

streamlit run app.py


After launching, the web interface will guide you through input fields for building characteristics and display estimated Heating and Cooling Loads.

Requirements

All necessary Python packages are listed in requirements.txt. Install them using the command above.

Acknowledgments

Special thanks to the creators and contributors of the Energy Efficiency dataset at the UCI Machine Learning Repository for providing such a valuable benchmark dataset for research and educational purposes
