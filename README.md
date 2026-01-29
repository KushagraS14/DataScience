Country Profile Variables Dataset Analysis
📊 Dataset Overview
This project analyzes the Country Profile Variables dataset containing socio-economic, environmental, and developmental indicators for 229 countries/regions across 50 different metrics.

📁 Dataset Information
Rows: 229 (countries/regions)

Columns: 50 (various indicators)

Size: 229 entries × 50 columns

Memory Usage: 89.6+ KB

🏗️ Data Structure
The dataset contains three main data types:

float64: 8 columns (continuous numerical values)

int64: 8 columns (integer numerical values)

object: 34 columns (mixed types including strings and numerical values stored as text)

🧹 Data Quality Assessment
✅ No missing values: All columns show 0 null entries

✅ No duplicates: 0 duplicated rows found

⚠️ Data type issues: 34 columns stored as objects that may need conversion for numerical analysis

⚠️ Placeholder values: "-99" appears frequently, likely representing missing/NA data

📈 Key Variables Analyzed
The analysis focused on "Population in thousands (2017)" as a primary variable:

Central Tendency Measures:
Mean: 32,756.79 thousand

Median: 5,448 thousand

Mode: Multiple modes present, highest frequency at 2,930 thousand

Dispersion Measures:
Range: 1,409,516 thousand

Standard Deviation: 133,275.08 thousand

Variance: 17,762,246,925.95

Interquartile Range (IQR): 18,762 thousand

Distribution Characteristics:
Q1 (25th percentile): 431 thousand

Q2 (50th percentile): 5,448 thousand

Q3 (75th percentile): 19,193 thousand

Outlier Detection:
Lower Fence: -27,712 thousand

Upper Fence: 47,336 thousand

Outliers Identified: 29 countries with populations exceeding upper fence

🔍 Correlation Analysis
A correlation matrix was generated for all numerical columns, revealing:

Strong positive correlation between population and CO2 emissions (0.70)

Moderate correlation between GDP and population (0.56)

Population density shows positive correlation with GDP per capita (0.48)

Several variables show no significant correlation with population

📊 Visualizations Created
Boxplots: For all numerical columns to identify outliers and distribution patterns

Heatmap: Correlation matrix visualization with annotation values

Statistical Summary: Complete descriptive statistics for numerical variables

🛠️ Technical Implementation
Libraries Used: NumPy, Pandas, Matplotlib, Seaborn

Data Loading: CSV file import with proper encoding

Analysis: Statistical calculations, outlier detection, correlation analysis

Visualization: Customized plots with appropriate formatting

📋 Data Cleaning Notes
The dataset appears pre-cleaned with no null values, but requires attention to:

Convert object-type columns to appropriate numerical formats

Handle "-99" placeholder values

Normalize column names for easier referencing

Address mixed data types in composite columns (e.g., "Urban population (% of total population)")

🎯 Potential Applications
This dataset supports analysis in:

Economic Development Studies

Environmental Impact Assessment

Public Health Research

Education System Comparisons

Infrastructure Planning

⚠️ Limitations
Mixed data types: Several columns contain combined metrics (e.g., ratios separated by "/")

Placeholder values: "-99" may skew statistical calculations

Year specificity: Most data is from 2017, limiting temporal analysis

Regional aggregation: Some data may be aggregated at regional levels

📈 Next Steps
Convert object columns to appropriate data types

Handle "-99" values systematically

Separate composite columns into individual metrics

Conduct region-specific analysis

Perform time-series analysis with historical data

Build predictive models for key development indicators

📚 Data Source
The dataset appears to be compiled from various UN and World Bank sources, providing a comprehensive country profile for comparative analysis.
