# Data Analysis and Visualization of Global Superstore Dataset

A comprehensive data analysis project exploring the Global Superstore dataset through preprocessing, visualization, and machine learning techniques.

## 📊 Project Overview

This project performs end-to-end data analysis on the Global Superstore dataset, including:
- Data cleaning and preprocessing
- Exploratory data analysis with visualizations
- Machine learning models for classification, prediction, and clustering
- Interactive Tableau dashboard

## 📁 Project Structure

```
├── Global_Superstore.csv                    # Original dataset
├── Global_Superstore_Preprocessed.csv       # Cleaned dataset
├── data_preprocessing.ipynb                 # Data cleaning notebook
├── data_visualization.ipynb                 # EDA and visualizations
├── ML_Analysis.ipynb                        # Machine learning models
├── Book1.twb                                # Tableau workbook
└── DAV innovative.docx                      # Project documentation
```

## 🔧 Technologies Used

- **Python 3.x**
- **Libraries:**
  - pandas - Data manipulation
  - numpy - Numerical operations
  - matplotlib & seaborn - Data visualization
  - scikit-learn - Machine learning models
- **Tableau** - Interactive dashboards

## 📈 Dataset Information

The Global Superstore dataset contains:
- **51,290 rows** of transaction data
- **24 columns** including:
  - Order details (Order ID, Date, Ship Mode)
  - Customer information (ID, Name, Segment)
  - Location data (City, State, Country, Region)
  - Product details (Category, Sub-Category, Product Name)
  - Financial metrics (Sales, Profit, Discount, Shipping Cost)

## 🛠️ Data Preprocessing

The preprocessing pipeline includes:

1. **Missing Value Handling**
   - Postal Code: 41,296 missing values filled with 'Unknown'

2. **Data Type Conversions**
   - Order Date and Ship Date converted to datetime format

3. **Feature Engineering**
   - Shipping_Days: Calculated delivery time
   - Order_Year, Order_Month, Order_Quarter: Temporal features
   - Profit_Margin: Percentage profit calculation
   - Profit_Category: Categorized profit levels (Loss, Low, Medium, High)

4. **Data Quality Checks**
   - Duplicate detection and removal
   - Outlier identification using IQR method
   - Data validation (negative quantities, invalid discounts)

## 📊 Visualizations

The project includes various visualizations:
- Distribution plots for numerical variables
- Category-wise sales and profit analysis
- Time series analysis
- Geographic distribution maps
- Correlation heatmaps
- Customer segment analysis

## 🤖 Machine Learning Models

### 1. Classification - Profit Category Prediction
- **Model:** Decision Tree Classifier
- **Accuracy:** 84.89%
- **Features:** Sales, Quantity, Discount, Shipping Cost, Category, Segment, Ship Mode
- **Target:** Profit_Category (Loss, Low Profit, Medium Profit, High Profit)

### 2. Regression - Sales Prediction
- **Model:** Linear Regression
- **Features:** Quantity, Discount, Shipping Cost, encoded categorical variables

### 3. Clustering - Customer Segmentation
- **Model:** K-Means Clustering
- **Purpose:** Identify customer groups based on purchasing behavior

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas numpy matplotlib seaborn scikit-learn jupyter
```

### Running the Notebooks

1. **Data Preprocessing:**
   ```bash
   jupyter notebook data_preprocessing.ipynb
   ```

2. **Data Visualization:**
   ```bash
   jupyter notebook data_visualization.ipynb
   ```

3. **Machine Learning Analysis:**
   ```bash
   jupyter notebook ML_Analysis.ipynb
   ```

## 📊 Key Insights

- Average sales per transaction: $246.49
- Average profit margin: 11.6%
- Most profitable category: Technology
- Peak sales period: Q4 (October-December)
- Customer segments: Consumer (51%), Corporate (30%), Home Office (19%)

## 📝 Results

The analysis reveals:
- Strong correlation between discount rates and profit margins
- Seasonal trends in sales patterns
- Geographic variations in product preferences
- Customer segmentation insights for targeted marketing

## 👥 Author

Sarth00718

## 📄 License

This project is open source and available for educational purposes.

## 🙏 Acknowledgments

- Dataset source: Global Superstore
- Inspired by real-world retail analytics challenges
