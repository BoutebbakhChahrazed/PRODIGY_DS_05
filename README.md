# Traffic Accident Data Analysis 🚗💥
### Prodigy InfoTech Data Science Internship - Task 05

## 📌 Project Overview
This project analyzes a countrywide traffic accident dataset to discern patterns and correlations between road conditions, weather, time of day, and accident severity. The analysis visualizes accident hotspots and contributing factors to provide insights into road safety.

The primary goal is to perform Exploratory Data Analysis (EDA) to understand:
*   **Time Analysis:** When accidents occur most frequently.
*   **Weather Analysis:** How weather impacts accident frequency.
*   **Geospatial Analysis:** Where accidents are most concentrated (hotspots).

## 📂 Dataset
*   **Source:** [US Accidents (March 2023) on Kaggle](https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents)
*   **Description:** A countrywide traffic accident dataset covering the United States (approx. 7.7 million records).
*   **File Used:** `US_Accidents_March23.csv`
*   *Note: Due to the file size, the dataset is not included in this repository. Please download it from the link above and place it in the input directory.*

## 🛠️ Technologies & Libraries Used
*   **Python 3**
*   **Pandas:** For data manipulation and cleaning.
*   **NumPy:** For numerical operations.
*   **Matplotlib & Seaborn:** For data visualization.

## 📊 Key Analysis Steps

### 1. Data Cleaning & Preparation
*   Loaded the dataset using Pandas.
*   Converted `Start_Time` and `End_Time` columns to datetime objects, handling inconsistent formats.
*   Selected relevant columns (`ID`, `Severity`, `Start_Time`, `Weather_Condition`, `Visibility`, `State`, `City`) to optimize memory usage.

### 2. Temporal Analysis
*   Extracted features like **Hour**, **Weekday**, and **Month** from timestamps.
*   **Insight:** Visualized accident frequency by hour of the day to identify peak traffic risk times (e.g., morning and evening rush hours).

### 3. Weather & Road Conditions
*   Analyzed the top 10 most frequent weather conditions present during accidents.
*   Created visibility bands (e.g., <0.5 mi, 0.5-2 mi) to observe the relationship between low visibility and accident severity.

### 4. Geospatial Analysis (Hotspots)
*   Grouped data by **State** and **City** to count accident occurrences.
*   Visualized the **Top 20 Cities** with the highest number of accidents to identify major hotspots.

## 📈 Visualizations Included
*   **Accidents by Hour of Day:** Bar chart showing peak accident times.
*   **Top 10 Weather Conditions:** Bar chart displaying the most common weather during crashes.
*   **Top 20 Accident Hotspots by City:** A breakdown of the most dangerous cities for driving.

## 🚀 How to Run
1.  Clone this repository.
2.  Ensure you have the dataset `US_Accidents_March23.csv` in the correct directory (update path in notebook if necessary).
3.  Install the required dependencies:
    ```
    pip install pandas numpy matplotlib seaborn
    ```
4.  Open the Jupyter Notebook:
    ```
    jupyter notebook prodigy-ds-05.ipynb
    ```
5.  Run all cells to generate the analysis and visualizations.

## 📜 License
This project is created for educational purposes as part of the Prodigy InfoTech Data Science Internship. The dataset is subject to its original license on Kaggle.
