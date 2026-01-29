# Regression for Energy Prediction

This project demonstrates the implementation of a **supervised learning procedure** to predict the energy requirements of a **machining (milling) process**. By using machine learning, the goal is to create transparency in energy planning, optimise process parameters, and enable effective load management.

## Project Overview
The core objective is to perform a regression analysis to forecast the energy needed for a milling process based on planned process parameters. The project follows a complete machine learning pipeline, from data pre-processing to model deployment.

### Key Features and Dataset
The model utilises data gathered from tests on a milling machine, controlled along three axes (X, Y, and Z). The dataset contains the following variables:
*   **Independent Variables (Features):** Axis (1–3), Feed (mm/min), and Path (mm).
*   **Target Variable:** Energy requirement in kilojoules (kJ).

### Technologies Used
*   **Language:** Python
*   **Libraries:** NumPy, Pandas, Matplotlib, Seaborn, and Scikit-learn.
*   **Environment:** Google Colab.

## Workflow
1.  **Data Loading & Statistical Analysis:** Importing data and performing initial statistical descriptions (mean, standard deviation, etc.).
2.  **Visualisation:** Using histograms to identify patterns, trends, and errors in the input data.
3.  **Data Cleaning:** 
    *   **Handling Missing Values:** Removing rows containing NaN values using `dropna()`.
    *   **Outlier Removal:** Filtering data to ensure values stay within realistic machining ranges (e.g., Axis: 1 to 3, Path: -60 to 60 mm, Feed: 500 to 3000 mm/min).
4.  **Dataset Splitting:** Dividing data into a **training set (75%)** to determine model parameters and a **test set (25%)** to evaluate performance on unseen data.
5.  **Model Implementation:** Training and testing three different regression algorithms:
    *   **Linear Regression**
    *   **Random Forest Regressor** (using 1000 decision trees)
    *   **Support Vector Regression (SVR)**
6.  **Evaluation:** Comparing models using **Mean Square Error (MSE)** and **Mean Absolute Error (MAE)**.
7.  **Deployment:** Using the best-performing model to predict energy for specific production settings.

## Results
A comparison of the models shows that the **Random Forest Regressor is the most accurate** for this dataset, as it produced the smallest error values. The Linear Regression and Support Vector Regression models showed significantly higher errors in comparison. 

*Note: In the context of this project, "parameters" are determined during training (e.g., weights), while "hyperparameters" (e.g., the number of trees in a Random Forest) are adjusted to optimise performance.*
===Project#1  Supervised Learning: Using different Regression Models for Energy prediction

Energy requirement for the milling process was predicted using three different models i.e. Linear Regression, Support Vector Machines, and Random Forest Generator. 
Different errors were calculated and all models were compared. 

​**Google Collab environment was used and many Python libraries such as Scikitlearn, Keras, Tenser Flow were implemented in both projects. Further information is given in below links.


--https://colab.research.google.com/drive/16fyqszTYamwr-aNvwoVoXkXdrXjKHWD9?usp=sharing (Project # 1)

## I used VS code, Python to push the files to my GitHub Repository.
## Also, you can use the above-provided link to check the Google Collab Notebook.

