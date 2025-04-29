# PE04 – Data Visualization in Python
**CS506 Programming for Computing**  
**City University of Seattle (CityU)**  

## Overview

This lab explores basic data visualization techniques using the `pandas` and `matplotlib` libraries in Python.  
The dataset `PE04_winereview.csv` contains 129,971 wine reviews. We focus on analyzing and plotting the frequency of values in the `points` and `price` columns.

---

## Part 1: Bar Chart using `value_counts()`

- Used `value_counts()` on the `"points"` column to count the frequency of each score.
- Created a bar chart using `.plot(kind='bar')`.
- Included a title and axis labels for clarity.
- The X-axis shows wine review scores, and the Y-axis shows the frequency.

---

## Part 2: Histogram of `"points"` with Bin Sizes 10 and 3

- Used `plt.hist()` to plot histograms for the `"points"` column.
- Two separate plots were created:
  - One with **bin size = 10**
  - One with **bin size = 3**
- Included title, X/Y axis labels, and grid lines.
- Restricted the X-axis range to 75–105 using `plt.xlim(75, 105)` for better readability.

---

## Part 3: Histogram of `"price"` with Bin Size 5

- Cleaned the `"price"` column using `pd.to_numeric(..., errors='coerce')` to convert and drop NaNs.
- Plotted a histogram using `plt.hist()` with **bin size = 5**.
- Restricted the X-axis to 0–550 using `plt.xlim(0, 550)` to minimize the effect of outliers.
- Included title, axis labels, and grid lines.

---

## Notes

- All visualizations used `matplotlib.pyplot` for plotting.
- Data was cleaned before plotting to remove missing or non-numeric values.
- Each graph was labeled clearly for readability.
