#  Running Analysis 🏃‍♂️

## 📊 Project Overview
This project analyzes over **600 running activities** collected over a period of nearly **5 years**. The dataset, extracted from a Garmin device, includes key metrics like distance, time, heart rate, elevation gain, calories burned and much more. Using Python’s libraries, this analysis uncovers patterns in training habits, running intensity, and performance.

The analysis explores:
- Temporal trends (when runs are most frequent)
- Key performance metrics (distance, speed, elevation, etc.)
- Identification of running streaks and breaks
- KMeans clustering to categorize runs by intensity

## 🛠️ Technologies Used
- **Python** (Programming language)
- **Pandas** (Data manipulation and analysis)
- **Matplotlib & Seaborn** (Data visualization)
- **Scikit-learn** (Machine learning - KMeans clustering)
- **Jupyter Notebook** (For code execution and visualization)

## 📂 Project Files

- **[`Activities.csv`](https://github.com/kostaskes/my-garmin-runs/blob/main/Activities.csv)**  
  Raw data file exported from Garmin Connect. Contains all activity types including running, cycling, and more.

- **[`running_activities.csv`](https://github.com/kostaskes/my-garmin-runs/blob/main/running_activities.csv)**  
  Filtered dataset including only running-related activities (`Running`, `Trail Running`, `Treadmill Running`).

- **[`running_analysis.ipynb`](https://github.com/kostaskes/my-garmin-runs/blob/main/running_analysis.ipynb)**  
  Jupyter Notebook with the complete analysis, visualizations, and clustering logic.

- **`README.md`**  
  Project overview, instructions, and documentation.


## 📈 Key Analyses Performed

### 1. Data Preparation & Cleaning
- **Date Conversion**: The 'Date' column was converted to the `datetime` format to ensure proper handling.
- **Temporal Features**: Additional columns were derived to capture year, month, day of week, time of day, and more.
- **Handling Missing Data**: Missing values in key numeric columns.
- **Unit Normalization**: Certain columns were scaled for machine learning purposes (e.g., converting time to minutes).

### 2. Running Activity Insights
- **Total Metrics**:
  - **Total Distance**: The overall distance covered across all running activities.
  - **Total Time**: Total time spent running, aggregated across all runs.
  - **Elevation Gain**: Total ascent during runs.
  - **Calories Burned**: The total number of calories burned.
- **Streaks & Breaks**:
  - The longest streak of consecutive running days and the longest break between runs was identified.

### 3. Temporal Analysis of Runs
- **Run Distribution**: The frequency of runs was analyzed by:
  - **Month**: Seasonal running trends and frequency.
  - **Day of Week**: Identifying preferred days of the week for runs.
  - **Time of Day**: Discovering peak hours of the day when runs tend to occur.
- **Peak Hours & Days**: The most common times and days for running were identified using bar charts.

### 4. Performance Clustering
- **KMeans Clustering**: 
  - Runs were grouped into 3 clusters based on **distance**, **average speed**, **heart rate**, and other features.
  - The clusters were labeled as:
    - **Easy Runs - Low Intensity**
    - **Moderate Runs - Medium Intensity**
    - **Hard Runs - High Intensity**
- **Clustering Insights**: The clustering analysis helped categorize different types of runs, providing a clearer picture of performance and effort levels.

## 📊 Key Visualizations

1. **Monthly Running Frequency**  
   A line chart showing how the number of runs fluctuates over time, highlighting peaks and dips in running activity.

2. **Hourly Distribution of Runs**  
   A bar chart visualizing the number of runs conducted at each hour of the day. The most common and least common hours for runs were highlighted.

3. **Clustering Visualization (Distance vs. Avg Speed)**  
   A scatter plot showing the relationship between the distance and average speed of runs, colored by cluster to visualize different run intensities.

4. **Day of Week Distribution**  
   A bar chart visualizing the number of runs by day of the week, helping to identify trends in which days of the week are preferred for running.

## 🎯 Project Goals
- Understand personal running patterns and habits over a 5-year period.
- Identify different types of runs (easy, moderate, hard) using KMeans clustering.
- Analyze key performance metrics (e.g., distance, calories, heart rate) and how they relate to running time and intensity.
- Provide insights into optimal training times, preferred running days, and intensity trends.

## 🔗 Project Code

Explore the complete code and analysis in the Jupyter notebook here👉[ running_analysis.ipynb ](https://github.com/kostaskes/my-garmin-runs/blob/main/running_analysis.ipynb)

---

🔗 **Explore more projects**: [github.com/kostaskes](https://github.com/kostaskes)


