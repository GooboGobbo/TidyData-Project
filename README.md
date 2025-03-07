# 🏅 2008 Olympic Medalists - Tidy Data Project

## 📌 Project Overview
This project focuses on cleaning and visualizing the 2008 Olympic medalist dataset using **tidy data principles**. The raw dataset contains unstructured information, requiring transformations to make it easier to analyze.

### **What is Tidy Data?**
Tidy data follows three key principles:
1. **Each variable** forms its own **column**.
2. **Each observation** forms its own **row**.
3. **Each value** belongs to its respective **cell**.

By applying these principles, we transform messy data into a structured format suitable for analysis and visualization.

---

## 🚀 How to Run This Project
### **1️⃣ Install Dependencies**
Ensure you have **Python 3.7+** and the required packages installed. You can install them using:
```sh
pip install streamlit pandas
```
### **2️⃣ Run the Streamlit App**
Clone the repository and navigate to the project folder. Then, run the following command:
```sh
streamlit run tidy_data_analysis.py
```
## Dataset Description
The dataset used in this project is from the 2008 Olympics, containing information about the athletes, their events, and medals (Gold, Silver, Bronze). The raw data was initially messy, with each athlete listed for every event, whether they participated or not.

### Preprocessing Steps:
1. **Data Melting**: The dataset was reshaped using the `melt()` function, so each row now represents a single athlete's performance in a specific event, with columns for the athlete, event, and medal.
2. **Column Splitting**: The `Event` column was split into two new columns, `Gender` and `Event`, to provide better clarity on the athlete's participation.
3. **Data Cleaning**: We removed any duplicate rows and dropped entries with missing values to ensure only complete data is used.
4. **Capitalization**: All textual columns (e.g., `Medal`, `Gender`, `Event`) were capitalized for consistency.

---

## Key Features of the Streamlit App
1. **Raw Data Preview**: Display the first few rows of the raw dataset to give users a sense of the unclean data.
2. **Melted Data Preview**: Show the transformed data where each row represents one medal achievement per athlete per event.
3. **Data Cleaning**: Demonstrate how data was cleaned, including splitting the `Event` column and capitalizing text fields.
4. **Medal Count by Event and Gender**: Use a pivot table and a bar chart to display the number of medals earned in each event, separated by gender.
5. **Athlete Achievement Exploration**: Allow users to select an athlete and see which events they participated in and what medals they won.
6. **Gender and Event Filtering**: Provide dropdown menus for users to filter the medalists by gender and event, displaying the athletes' names and the medals they won.

