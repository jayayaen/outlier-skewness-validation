## Outlier and Skewness Validation Pipeline
This project provides a robust, production-ready Python pipeline to **detect and address skewness and outliers** in numeric datasets. <br/>
It is designed to streamline the data validation process before statistical analysis or machine learning model development.


A clean, PEP8-compliant Python pipeline to:
- Detect skewed features
- Apply log1p transformation
- Define safe value ranges
- Validate and log outliers
- Generate visual boxplots

### What Does This Code Do?

This pipeline:
1. **Identifies highly skewed numeric features** using statistical skewness
2. **Applies `np.log1p` transformation** to reduce skew
3. **Defines safe ranges** using either percentiles or fixed buffer
4. **Validates values** for each feature against defined bounds
5. **Logs outliers** to CSV files (raw + sparse format)
6. **Generates visual boxplots** for inspection
7. **Outputs a summary** of all validations

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
