#  Bangalore House Prices – Outlier Detection and EDA

This project explores house price data in Bangalore with a focus on **price per square foot**. The goal is to detect and remove outliers using various statistical methods and perform exploratory data analysis (EDA) to better understand the dataset.

## 📁 Dataset

- **Source**: [house_price.csv](https://drive.google.com/file/d/1UlWRYU0UglE2ex3iFse0J6eCLEU8g98P/view?usp=sharing)
- **Columns**:
  - `location`: Area of the property
  - `size`: Number of bedrooms or configuration (e.g., 2 BHK)
  - `total_sqft`: Total area in square feet
  - `bath`: Number of bathrooms
  - `price`: Price in lakhs
  - `bhk`: Number of bedrooms
  - `price_per_sqft`: Calculated price per square foot

##  Project Tasks

### Q1.  Basic EDA :
- Dataset overview
- Data types and missing values
- Summary statistics
- Sample rows

### Q2. Outlier Detection & Removal :

Applied on the `price_per_sqft` column using:
1. **Mean ± 3×Std Dev**
2. **Percentile Method (5th to 95th)**
3. **IQR (Interquartile Range)**
4. **Z-Score Method**

Methods used for handling:
- **Trimming**: Removing the rows with extreme values.

### Q3. Box Plot Comparison :
- Box plots for each method to visually assess which outlier removal technique is most effective.

### Q4. Normality Check :
- Histograms before and after transformation.
- Applied **log transformation** to correct skewness.
- Measured:
  - **Skewness**
  - **Kurtosis**

### Q5. Correlation Heatmap :
- Analyzed numerical features using correlation matrix.
- Visualized with a **Seaborn heatmap**.

### Q6. Scatter Plots :
- Scatter plots between `price_per_sqft` and other numeric features like `total_sqft`, `bath`, and `bhk`.


## Result Summary :

| Method          | Rows Retained |
|-----------------|----------------|
| Mean ± Std Dev  | 13,195         |
| Percentile      | 11,880         |
| IQR             | 11,935         |
| Z-Score         | 13,195         |

✅ **Best Method**: IQR or Percentile, based on box plot and histogram analysis.


## References :

- YouTube: [Outlier Detection Tutorial](https://youtu.be/Cw2IvmWRcXs?si=KYjsr1vThZNNrDUr)
