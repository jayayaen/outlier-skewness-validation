## Outlier and Skewness Validation Pipeline
Python pipeline to detect and transform skewed features, validate outliers, and produce logs and plots.


A clean, PEP8-compliant Python pipeline to:
- Detect skewed features
- Apply log1p transformation
- Define safe value ranges
- Validate and log outliers
- Generate visual boxplots

### What Does This Code Do?

This pipeline:
1. Identifies highly skewed numeric features using statistical skewness.
2. Applies `np.log1p` transformation to reduce skew (handle non-normal distributions).
3. Defines safe ranges for each feature using percentiles (1st to 99th).
4. Validates each feature’s values against these ranges.
5. Logs outliers (in full and sparse format) to CSV files.
6. Generates boxplots for visual inspection of each feature.
7. Produces a summary report of outlier counts per feature.

This helps ensure your numeric features are:
- More normally distributed (for modeling),
- Free from extreme outliers (for analysis or visualization),
- Well-documented with visual and CSV-based reporting.

### Files
- `outlier_skew_validation.py`: Full pipeline script
- `README.md`: This documentation

### Usage
1. Place your dataset as `Wisconsin_Breast_Cancer_Dataset.csv` in the working directory.
2. Run the script.
3. Review the outlier logs and validation summary.

### Dependencies
- Python 3.x
- numpy
- pandas
- seaborn
- matplotlib
- scipy

### Output
- Outlier logs (per feature)
- Combined outlier CSV
- Boxplots for visual validation

 For medical, finance, or ML applications — plug in your dataset and go!

Author - Jayanthan Jayaratnam <br/>
[LinkedIn](https://www.linkedin.com/in/aj41/) | [GitHub](https://github.com/jayayaen)
