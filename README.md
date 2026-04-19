# 🍽️ Restaurant Data Analysis

A comprehensive exploratory data analysis (EDA) project on restaurant data sourced from the **Cognifyz Technologies Dataset**, uncovering trends in cuisines, ratings, pricing, online delivery, and customer engagement across global restaurant markets.

---

## 📌 Table of Contents

- [Project Overview](#project-overview)
- [Dataset Description](#dataset-description)
- [Project Structure](#project-structure)
- [Key Objectives](#key-objectives)
- [Analysis Highlights](#analysis-highlights)
- [Technologies Used](#technologies-used)
- [Setup & Usage](#setup--usage)
- [Results & Insights](#results--insights)

---

## 📖 Project Overview

This project analyzes a rich dataset of **9,551 restaurants** spanning multiple countries and cities. The goal is to derive actionable insights about restaurant trends, customer preferences, cuisine popularity, pricing strategies, and the impact of services like online delivery and table booking on ratings.

---

## 📊 Dataset Description

**Source:** Cognifyz Technologies Dataset  
**File:** `data/Cognifyz Technologies Dataset.csv`  
**Shape:** 9,551 rows × 21 columns (9,542 rows × 13 columns after cleaning)

### Column Reference

| # | Column | Description |
|---|--------|-------------|
| 1 | Restaurant ID | Unique identifier for each restaurant |
| 2 | Restaurant Name | Name of the restaurant |
| 3 | Country Code | Numeric code representing the country |
| 4 | City | City where the restaurant is located |
| 5 | Address | Full address of the restaurant |
| 6 | Locality | Specific area or neighborhood |
| 7 | Locality Verbose | Detailed locality with city |
| 8 | Longitude | Geographic longitude coordinate |
| 9 | Latitude | Geographic latitude coordinate |
| 10 | Cuisines | Types of cuisines offered |
| 11 | Average Cost for Two | Estimated cost for two people |
| 12 | Currency | Currency used for pricing |
| 13 | Has Table Booking | Whether table booking is available (Yes/No) |
| 14 | Has Online Delivery | Whether online delivery is offered (Yes/No) |
| 15 | Is Delivering Now | Whether restaurant is currently delivering |
| 16 | Switch to Order Menu | Alternative order menu availability |
| 17 | Price Range | Pricing category (1–4) |
| 18 | Aggregate Rating | Overall customer rating (0–5 scale) |
| 19 | Rating Color | Color-coded rating (e.g., Dark Green = Excellent) |
| 20 | Rating Text | Textual rating (Excellent, Very Good, Average, etc.) |
| 21 | Votes | Number of customer votes received |

---

## 📁 Project Structure

```
Restaurant-Data-Analysis/
│
├── data/
│   └── Cognifyz Technologies Dataset.csv   # Raw dataset
│
├── notebooks/
│   └── Restaurant_Data_Analysis.ipynb      # Full analysis notebook
│
└── README.md                               # Project documentation
```

---

## 🎯 Key Objectives

1. **Cuisine Analysis** — Identify the most popular cuisines and percentage distribution
2. **City-wise Distribution** — Find cities with the highest restaurant concentration
3. **Rating Trends** — Analyze average ratings across cities and cuisine types
4. **Price Range Distribution** — Visualize how restaurants are distributed by pricing tier
5. **Online Delivery Impact** — Compare ratings of restaurants with/without delivery
6. **Customer Engagement** — Explore vote distribution and its correlation with ratings
7. **Restaurant Chains** — Identify and analyze major restaurant chains in the dataset
8. **Review Sentiment** — Examine the distribution of rating text categories

---

## 🔍 Analysis Highlights

### 🍛 Cuisine Insights
- **145 unique cuisines** are represented in the dataset
- **North Indian** leads with 20.09% share, followed by **Chinese (13.88%)** and **Fast Food (10.08%)**
- Top cuisine combinations: *North Indian* (936), *North Indian + Chinese* (511), *Chinese* (354)
- Cuisines consistently receiving high ratings: **Cafe, North Indian, Italian, Mughlai**

### 🏙️ City-wise Distribution
- **New Delhi** has the highest number of restaurants — **5,473**
- **Inner City** holds the highest average rating of **4.90**

### 💰 Price Range Distribution
| Price Category | Restaurants | Percentage |
|----------------|-------------|------------|
| Low Price | 4,444 | 46.5% |
| Medium-Low Price | 3,113 | 32.6% |
| Medium-High Price | 1,408 | 14.7% |
| High Price | 586 | 6.1% |

> 💡 The majority (46.5%) of restaurants are budget-friendly, reflecting strong demand for affordable dining.

### 🚴 Online Delivery Impact
- Only **25.6%** of restaurants offer online delivery
- Restaurants **with** online delivery: ⭐ Avg Rating **3.2**
- Restaurants **without** online delivery: ⭐ Avg Rating **2.4**

> 💡 Online delivery is positively correlated with higher customer ratings.

### 🗳️ Customer Engagement
- **Average votes** per restaurant: **156.8**
- **Highest votes** received: **10,934** (Toit Restaurant)
- **1,094 restaurants** have 0 votes — indicating low visibility
- Weak positive correlation (0.31) between votes and aggregate rating

### 🏪 Top Restaurant Chains
| Chain | Outlets |
|-------|---------|
| Cafe Coffee Day | 83 |
| Domino's Pizza | 79 |
| Subway | 63 |
| Green Chick Chop | 51 |
| McDonald's | 48 |

### ⭐ Rating Distribution
| Rating | Count |
|--------|-------|
| Average | 3,734 |
| Not Rated | 2,148 |
| Good | 2,096 |
| Very Good | 1,078 |
| Excellent | 300 |
| Poor | 186 |

> 💡 Most restaurants receive "Average" ratings — indicating significant room for service improvement.

---

## 🛠️ Technologies Used

| Tool | Purpose |
|------|---------|
| **Python 3.x** | Core programming language |
| **Pandas** | Data loading, cleaning, and manipulation |
| **NumPy** | Numerical computations |
| **Matplotlib** | Static data visualizations |
| **Seaborn** | Statistical plotting and styling |
| **Jupyter Notebook** | Interactive analysis environment |

---

## ⚙️ Setup & Usage

### Prerequisites

Ensure you have Python 3.7+ installed. Install the required dependencies:

```bash
pip install pandas numpy matplotlib seaborn jupyter
```

### Running the Analysis

1. **Clone the repository:**
   ```bash
   git clone https://github.com/anuragsathe/Restaurant-Data-Analysis.git
   cd Restaurant-Data-Analysis
   ```

2. **Launch the Jupyter Notebook:**
   ```bash
   jupyter notebook notebooks/Restaurant_Data_Analysis.ipynb
   ```

3. **Run all cells** to reproduce the full analysis and visualizations.

> **Note:** The dataset is located at `data/Cognifyz Technologies Dataset.csv`. The notebook references this path — ensure the directory structure is maintained.

---

## 📈 Results & Insights

- **North Indian cuisine dominates** the market, driven by regional preferences in India, which has the largest share of restaurants in the dataset.
- **Budget-friendly restaurants** account for nearly half of all listings, emphasizing the mass-market segment.
- **Online delivery is an emerging differentiator** — restaurants offering it tend to have significantly higher ratings, suggesting customer satisfaction is linked to accessibility and convenience.
- **Restaurant chains like Cafe Coffee Day and Domino's** have the widest reach, highlighting strong brand penetration in the quick-service and café segments.
- **Customer engagement (votes) weakly correlates with ratings**, suggesting popularity is tied to multiple factors beyond just quality.

---

## 📝 License

This project is for educational and internship purposes. Dataset provided by **Cognifyz Technologies**.

---

*Developed as part of the **Cognifyz Technologies Data Analysis Internship** program.*