# 18_202401100400131
Healthcare Data Cleaning: Improve disease prediction accuracy by handling missing,  inconsistent, and noisy patient data.
Healthcare Data Cleaning Project
Overview


This project cleans a synthetic healthcare dataset by handling missing values, inconsistencies, and outliers to improve disease prediction accuracy. The cleaned dataset ensures reliable data for analysis and machine learning models.

What This Project Does


Generates patient data (ID, Age, Blood Pressure, Cholesterol, Disease).
Handles missing values using statistical imputation.
Fixes inconsistent disease names to maintain uniformity.
Detects and removes outliers using the Z-score method.
Visualizes data distribution with boxplots.
Saves the cleaned dataset for further analysis.


Technologies Used

Python – Programming language.
Pandas – Data handling and processing.
NumPy – Numerical operations.
Matplotlib & Seaborn – Data visualization.
SciPy – Statistical analysis for outlier detection.


Functions Used in the Code

1. Generate Synthetic Data
python
Copy
Edit
def generate_healthcare_data(num_records=200):
Creates a random dataset of 200 patient records.
Adds random missing values for Blood Pressure and Cholesterol.
Introduces spelling errors in disease names to simulate inconsistencies.


2. Handle Missing Values
python
Copy
Edit
def handle_missing_values(df):
Replaces missing Blood Pressure values with the mean.
Replaces missing Cholesterol values with the median.


3. Fix Disease Name Inconsistencies
python
Copy
Edit
def standardize_disease_names(df):
Converts all disease names to lowercase.
Fixes spelling mistakes (e.g., "Hpertension" → "Hypertension").
Standardizes capitalization.


4. Remove Outliers
python
Copy
Edit
def remove_outliers(df):
Uses the Z-score method to identify and remove outliers.
Removes extreme values in Age, Blood Pressure, and Cholesterol.


5. Visualize Data Distribution
python
Copy
Edit
def visualize_data(df):
Creates a boxplot to detect outliers.
Shows the spread of Age, Blood Pressure, and Cholesterol.


How to Run the Code


1. Install Dependencies
Make sure you have Python installed, then run:

bash
Copy
Edit
pip install numpy pandas matplotlib seaborn scipy


2. Run the Script
bash
Copy
Edit
python healthcare_data_cleaning.py
This will clean the dataset and save it as cleaned_healthcare_data.csv.


3. View the Results
The script will generate a boxplot to visualize outliers.
The cleaned dataset will be stored in CSV format for further analysis.
Project Structure
bash
Copy
Edit
📂 Healthcare-Data-Cleaning
│── 📄 README.md  # Project documentation  
│── 📄 cleaned_healthcare_data.csv  # Cleaned dataset  
│── 📄 healthcare_data_cleaning.py  # Python script  
References
Pandas Documentation – Data handling functions.
Seaborn Documentation – Data visualization.
SciPy Documentation – Statistical functions for outlier removal.


Author
Nischhal Garg


License
This project is open-source and for educational purposes.


