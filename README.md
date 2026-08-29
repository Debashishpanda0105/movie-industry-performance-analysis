# 🎬 Movie Industry Performance Analysis Using Python & Pandas

> An end-to-end Data Analytics project analyzing movie production, audience engagement, financial performance, profitability, and ROI using Python and Pandas.

---

## 📌 Project Overview

This project analyzes a movie industry dataset containing information about movies, ratings, genres, release dates, audience engagement, budgets, gross revenue, directors, stars, countries, and production companies.

The objective is to transform raw movie data into meaningful, business-oriented insights using a complete data analytics workflow.

The project covers:

- Data Inspection
- Data Cleaning
- Data Validation
- Feature Engineering
- Exploratory Data Analysis
- Financial Analysis
- Data Visualization
- Business Insights
- Recommendations

---

## 🎯 Business Problem

Movie production requires significant financial investment and involves considerable business risk.

Production companies, investors, and decision-makers need to understand which factors are associated with successful movie performance.

This project aims to answer questions such as:

- Which movie genres perform strongly?
- Which movies generate the highest profit?
- Which movies achieve the highest ROI?
- How does production budget relate to gross revenue?
- How does audience engagement relate to movie performance?
- Which directors demonstrate strong historical performance?
- Which production companies perform well?
- How has movie production changed over time?
- Does higher investment necessarily lead to higher returns?

The goal is to use historical movie data to support data-driven decision making.

---

# 📊 Dataset

The dataset contains approximately **7,668 movies** and initially includes **15 columns**.

### Original Columns

| Column | Description |
|---|---|
| `name` | Movie name |
| `rating` | Movie rating classification |
| `genre` | Movie genre |
| `year` | Movie release year |
| `released` | Movie release date |
| `score` | Movie score |
| `votes` | Number of audience votes |
| `director` | Movie director |
| `writer` | Movie writer |
| `star` | Main star |
| `country` | Country of production |
| `budget` | Production budget |
| `gross` | Gross revenue |
| `company` | Production company |
| `runtime` | Movie runtime |

---

# ⚙️ Feature Engineering

Additional analytical features were created to support business analysis.

### Date Features

- `release_year`
- `release_month`
- `release_month_name`
- `release_quarter`
- `release_decade`

### Financial Features

- `profit`
- `roi`

### Business Categories

- `profit_status`
- `budget_category`
- `gross_category`
- `rating_category`

The final analytical dataset contains **26 columns**.

---

# 💰 Financial Metrics

## Profit

```text
Profit = Gross Revenue - Budget
```

## ROI

```text
ROI = (Profit / Budget) × 100
```

### Why Both Metrics Matter

**Profit** → Absolute financial gain

**ROI** → Investment efficiency

A movie can therefore generate high absolute profit without having the highest ROI.

Similarly, a low-budget movie can achieve a very high ROI while generating less absolute profit.

---

# 🧹 Data Cleaning

The raw dataset was inspected and validated for:

- Missing values
- Duplicate records
- Incorrect data types
- Invalid dates
- Negative financial values
- Potential outliers
- Inconsistent categorical data

### Key Cleaning Activities

- Converted release dates into datetime format
- Removed country information from release-date values
- Handled missing values
- Validated numerical data types
- Checked duplicate records
- Validated budget and gross values
- Investigated unusual runtime values
- Standardized categorical information

### Duplicate Check

```text
0 duplicate records
```

### Financial Validation

Budget and gross revenue were checked for negative values.

No negative financial values were identified.

---

# 🔍 Exploratory Data Analysis

The project performed exploratory analysis across multiple business dimensions.

## 📅 Time Analysis

- Movie production by year
- Movie production by decade
- Release trends
- Financial performance over time

## 🎬 Genre Analysis

- Genre distribution
- Genre movie count
- Genre revenue
- Genre profit
- Average genre performance
- Average genre score

## 💰 Financial Analysis

- Production budget
- Gross revenue
- Profit
- ROI
- Profit status
- Budget categories
- Revenue categories

## ⭐ Audience Analysis

- Movie scores
- Number of votes
- Audience engagement
- Rating categories

## 🎥 Performance Analysis

- Top profitable movies
- Top ROI movies
- Director performance
- Production company performance

---

# 📈 Data Visualization

Matplotlib was used to communicate important analytical findings.

Visualizations included:

- Movie production trends
- Genre comparisons
- Revenue comparisons
- Profit comparisons
- Budget analysis
- Top profitable movies
- Top ROI movies
- Decade performance
- Director performance
- Production company performance

### Visualization Principles

| Visualization | Purpose |
|---|---|
| Line Chart | Time trends |
| Bar Chart | Category comparison |
| Horizontal Bar Chart | Ranking |
| Scatter Plot | Relationship between numerical variables |

---

# 🧠 Business Insights

The analysis demonstrates that movie success cannot be evaluated using a single metric.

Important dimensions of movie performance include:

- Revenue
- Profit
- ROI
- Production Budget
- Audience Engagement
- Movie Score
- Genre
- Director
- Production Company
- Release Period

### Key Insight

A movie with the highest gross revenue is not necessarily the most efficient investment.

Likewise, a movie with the highest ROI is not necessarily the movie with the highest absolute profit.

Therefore, financial performance should be evaluated using multiple metrics.

---

# 🎯 Business Recommendations

### 1. Evaluate Profit and ROI Together

Use profit to understand absolute financial performance and ROI to understand investment efficiency.

### 2. Analyze Genre Performance

Historical genre performance can be considered when evaluating future movie opportunities.

### 3. Control Budget Risk

High-budget projects involve greater financial exposure.

Budget decisions should therefore be evaluated against expected revenue, profit, and ROI.

### 4. Consider Historical Performance

Director and production company performance can provide useful historical context when evaluating future projects.

### 5. Use Audience Metrics

Scores and votes can provide additional information about audience reception and engagement.

### 6. Avoid Single-Metric Decisions

Investment decisions should combine:

```text
Financial Performance
        +
Audience Performance
        +
Historical Performance
```

---

# 🔄 Project Workflow

```text
                 RAW DATA
                    │
                    ▼
          DATA INSPECTION
                    │
                    ▼
           DATA CLEANING
                    │
                    ▼
          DATA VALIDATION
                    │
                    ▼
       FEATURE ENGINEERING
                    │
                    ▼
            EDA / ANALYSIS
                    │
                    ▼
        FINANCIAL ANALYSIS
                    │
                    ▼
          VISUALIZATION
                    │
                    ▼
         BUSINESS INSIGHTS
                    │
                    ▼
          RECOMMENDATIONS
```

---

# 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| **Python** | Programming & analysis |
| **Pandas** | Data manipulation & analysis |
| **NumPy** | Numerical operations |
| **Matplotlib** | Data visualization |
| **Jupyter Notebook** | Development environment |

---

# 📁 Project Structure

```text
movie-industry-performance-analysis/
│
├── 📁 data/
│   └── movie_dataset.csv
│
├── 📁 notebooks/
│   └── Movie_Industry_Analysis.ipynb
│
├── 📁 visuals/
│   ├── movie_trends.png
│   ├── genre_analysis.png
│   ├── financial_analysis.png
│   └── top_movies.png
│
├── 📁 documentation/
│   ├── Business_Problem.md
│   ├── Data_Dictionary.md
│   └── Business_Insights.md
│
├── README.md
└── .gitignore
```

> **Dataset note:** Before uploading the original dataset to GitHub, verify the source dataset's license and redistribution terms. If redistribution is not permitted, keep the dataset local and mention the source in the project documentation.

---

# 🚀 How to Run the Project

## 1. Clone the Repository

```bash
git clone <repository-url>
```

## 2. Navigate to the Project

```bash
cd movie-industry-performance-analysis
```

## 3. Install Required Libraries

```bash
pip install pandas numpy matplotlib jupyter
```

## 4. Launch Jupyter Notebook

```bash
jupyter notebook
```

## 5. Open the Notebook

```text
notebooks/Movie_Industry_Analysis.ipynb
```

Run the notebook cells sequentially.

---

# 📚 Skills Demonstrated

### Python & Pandas

- DataFrame
- Series
- Data Cleaning
- Data Transformation
- GroupBy
- Aggregation
- Sorting
- Filtering
- Missing Value Handling
- Datetime Processing

### Data Analytics

- Exploratory Data Analysis
- Descriptive Statistics
- Feature Engineering
- Correlation Analysis
- Financial Analysis
- ROI Analysis
- Ranking Analysis
- Time-Series Analysis

### Data Visualization

- Matplotlib
- Trend Analysis
- Category Comparison
- Distribution Analysis
- Relationship Analysis

### Business Analytics

- KPI Analysis
- Profitability Analysis
- Investment Efficiency
- Business Insights
- Business Recommendations
- Data Storytelling

---

# ⚠️ Project Limitations

The analysis has several limitations:

- The dataset represents only the movies available in the source dataset.
- Some financial fields contain missing values.
- Historical performance does not guarantee future success.
- Gross revenue does not represent complete studio profitability.
- Marketing and distribution costs are not fully represented.
- ROI depends on the availability and quality of budget and gross revenue data.
- The dataset should not automatically be treated as a complete representation of the global movie industry.

Therefore, the findings should be interpreted as analytical insights rather than definitive predictions.

---

# 🏁 Final Conclusion

This project demonstrates a complete end-to-end data analytics workflow using Python and Pandas.

Starting from raw movie data, the project progressed through:

```text
Data Inspection
      ↓
Data Cleaning
      ↓
Feature Engineering
      ↓
Exploratory Data Analysis
      ↓
Financial Analysis
      ↓
Visualization
      ↓
Business Insights
      ↓
Recommendations
```

The analysis demonstrates that professional data analytics is not only about writing Python code.

A professional analyst must be able to:

1. Understand the business problem.
2. Inspect and clean the data.
3. Validate data quality.
4. Engineer meaningful features.
5. Explore patterns and relationships.
6. Select appropriate business metrics.
7. Visualize important findings.
8. Translate analysis into business insights.
9. Communicate recommendations clearly.

## Final Takeaway

Movie performance should be evaluated from multiple perspectives, including:

**Financial Return + Investment Efficiency + Audience Engagement + Historical Performance**

This project demonstrates how Python and Pandas can transform raw data into structured analysis and actionable business insights.

---

# 👤 Author

## Debashish Panda

**Aspiring Data Analyst**

### Core Skills

`Python` `Pandas` `SQL` `Power BI` `Excel` `Tableau`

---

⭐ If you found this project useful, consider giving the repository a star.
