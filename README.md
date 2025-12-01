# Pandas Data Science Practice - Titanic Dataset
# ok this is the git push
A beginner-friendly guide to data cleaning, exploration, and feature engineering using Python Pandas.

## Project Overview

This project demonstrates essential data science techniques for preparing and analyzing the Titanic dataset. Perfect for beginners learning data cleaning and pandas operations.

## Files in This Project

### 1. **Data science series pandas, numpy practice.ipynb**
The main beginner notebook covering:
- Loading CSV data
- Understanding dataset structure
- Handling missing values
- Basic data cleaning
- Preparing data for machine learning

**What you'll learn:**
- How to import and explore data
- Identifying and fixing null values
- Dropping columns with too many missing values
- Filling missing data with mean/median
- Splitting data into features (X) and target (y)

### 2. **Advanced_Pandas_Techniques.ipynb**
Advanced techniques for experienced users:
- Feature engineering (creating new features)
- GroupBy operations and aggregations
- Categorical encoding (Label & One-Hot)
- Outlier detection and handling
- Data visualization with matplotlib/seaborn
- Creating ML-ready datasets

**What you'll learn:**
- Extract features from text (titles from names)
- Create age groups and fare categories
- Analyze survival rates by different groups
- Detect and handle outliers
- Scale features for machine learning

### 3. **data_science_pandas_practice.py**
Python script version of the basic notebook for running in terminal or IDE.

### 4. **requirments.txt**
List of required Python packages.

## Dataset

**Titanic Test Dataset** (`tested.csv`)
- 418 passenger records
- 12 columns including: PassengerId, Survived, Pclass, Name, Sex, Age, Fare, etc.

## Installation

1. Clone or download this repository

2. Install required packages:
```bash
pip install -r requirments.txt
```

Required libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

## How to Use

### For Beginners:
1. Start with `Data science series pandas, numpy practice.ipynb`
2. Run cells sequentially to understand each step
3. Read the comments to learn what each operation does

### For Advanced Users:
1. After completing the basic notebook, open `Advanced_Pandas_Techniques.ipynb`
2. Explore feature engineering and advanced pandas operations
3. Learn visualization and outlier detection techniques

### Using Python Script:
```bash
python data_science_pandas_practice.py
```

## Key Concepts Covered

### Basic Notebook:
- `pd.read_csv()` - Load data
- `.head()`, `.tail()` - View data
- `.info()` - Dataset information
- `.isnull().sum()` - Count missing values
- `.fillna()` - Fill missing values
- `.drop()` - Remove columns
- `.describe()` - Statistical summary

### Advanced Notebook:
- `value_counts()` - Count categories
- `.groupby()` - Group and aggregate
- `pd.cut()`, `pd.qcut()` - Create bins
- `pd.get_dummies()` - One-hot encoding
- `.corr()` - Correlation analysis
- Outlier detection with IQR method
- Feature scaling with StandardScaler

## Data Cleaning Workflow

```
1. Import Dataset
   ↓
2. Explore Data (head, info, describe)
   ↓
3. Check Missing Values
   ↓
4. Handle Missing Data
   - Drop if > 50% missing (Cabin: 78% → dropped)
   - Fill with mean/median (Age, Fare)
   ↓
5. Feature Engineering (optional)
   - Create new features
   - Encode categories
   ↓
6. Split into X (features) and y (target)
   ↓
7. Ready for Machine Learning!
```

## Results

After cleaning:
- **0 missing values** in all columns
- **10 features** ready for modeling
- **418 complete records**
- Dataset split into features (X) and target (y)

## Tips for Beginners

1. **Always explore first** - Use `.head()`, `.info()`, `.describe()` before cleaning
2. **Handle missing data carefully** - Understand why data is missing
3. **Document your decisions** - Add comments explaining why you chose mean vs median
4. **Visualize your data** - Use plots to understand distributions
5. **Check after each step** - Verify your cleaning worked as expected

## Common Mistakes to Avoid

- Don't drop columns without checking how much data is missing
- Don't fill missing values without understanding the data distribution
- Don't forget to use `inplace=True` or reassign the variable
- Don't skip exploratory analysis
- Don't use deprecated syntax (use `axis=1` instead of positional arguments)

## Next Steps

After completing these notebooks:
1. Try applying these techniques to other datasets
2. Learn about train/test splitting
3. Build machine learning models (Logistic Regression, Decision Trees)
4. Explore cross-validation
5. Learn hyperparameter tuning

## Resources

- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [NumPy Documentation](https://numpy.org/doc/)
- [Scikit-learn Documentation](https://scikit-learn.org/)

## Author

Practice project for learning pandas and data science fundamentals.

## License

Free to use for educational purposes.

---

**Happy Learning!** Start with the basic notebook and work your way up to advanced techniques.
