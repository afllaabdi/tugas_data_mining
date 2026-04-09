# Indonesia Food Price Analysis & Clustering

This project analyzes food price data in Indonesia using data preprocessing, visualization, and clustering techniques.

The goal is to identify patterns and group similar price behaviors using unsupervised learning.

---

## Project Workflow

### 1. Data Loading

* Dataset loaded from Google Drive
* Initial inspection using Pandas

### 2. Data Cleaning

* Removed invalid date values
* Converted date column to datetime format
* Converted price to numeric
* Removed missing values and duplicates

### 3. Data Transformation

* Extracted year and month from date
* Prepared time-based features

### 4. Feature Selection

Selected relevant features:

* year, month
* location (admin1, market)
* category, commodity
* price

### 5. Encoding

* Applied Label Encoding to categorical variables

### 6. Data Visualization

* Correlation heatmap
* Price distribution histogram
* Monthly price trend analysis

### 7. Clustering (K-Means)

* Applied K-Means clustering (k=3)
* Grouped data based on price and features
* Visualized clusters
* Analyzed average price per cluster

---

## Key Insights

* Food prices show seasonal trends across months
* Certain commodities have distinct pricing patterns
* Clustering helps group similar market behaviors
* Price distribution is not uniform across regions

---

## Technologies Used

Python
Pandas
NumPy
Matplotlib
Seaborn
Scikit-learn

---

## Output

* Clustered dataset saved as CSV
* Visual insights from heatmap and trends
* Grouped price behavior using K-Means

---

## Future Improvements

* Use advanced clustering (DBSCAN, Hierarchical)
* Add geospatial analysis
* Build prediction model for price forecasting
* Create dashboard for real-time monitoring
