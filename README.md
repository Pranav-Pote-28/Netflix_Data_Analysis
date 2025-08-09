# 📊 Netflix EDA (Exploratory Data Analysis)

This project performs **Exploratory Data Analysis (EDA)** on a Netflix movie dataset to uncover trends, patterns, and insights related to genres, popularity, and ratings.

---

## 📂 Dataset Overview
- **Rows:** 9,827  
- **Columns:** 9 (after cleaning)  
- **Original Columns:** `Title`, `Overview`, `Original_Language`, `Poster_Url`, `Release_Date`, `Genre`, `Popularity`, `Vote_Average`, `Vote_Count`  
- **Key Notes from Data Exploration:**
  - No missing values or duplicates initially.
  - `Release_Date` converted to **year** only.
  - Dropped less useful columns: `Overview`, `Original_Language`, `Poster_Url`.
  - `Popularity` column contained noticeable outliers.
  - `Vote_Average` transformed into categories for analysis.
  - `Genre` column had comma-separated values, split into multiple rows and converted to category type.

---

## 🛠 Data Cleaning & Transformation Steps
1. **Removed Specific Rows:** Dropped rows from index 1106 to 1115.
2. **Date Conversion:** Converted `Release_Date` to datetime format, then extracted year.
3. **Column Removal:** Dropped non-essential columns.
4. **Vote Average Categorization:**
   - Created bins: `Not Popular`, `Below Average`, `Average`, `Popular`.
5. **Genre Processing:**
   - Split multi-genre movies into multiple rows.
   - Converted `Genre` to categorical type.
6. **Removed Remaining NaNs** after transformations.

---

## 📈 Analysis & Visualizations
### 1️⃣ Most Frequent Genre
- Count plot showing the top genres on Netflix.
  
### 2️⃣ Highest Vote Average Category
- Count plot of `Vote_Average` categories.

### 3️⃣ Most Popular Movie
- Identified movie with **highest popularity** and its genre.

### 4️⃣ Least Popular Movie
- Identified movie with **lowest popularity** and its genre.

### 5️⃣ Movie Releases by Year
- Histogram showing the year with the most movie releases.

---

## 📊 Tools & Libraries Used
- **Python** 🐍
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**

---

## 📷 Example Plots
- **Genre Distribution**
- **Vote Average Categories**
- **Release Year Distribution**

---

## 🚀 How to Run
1. Clone this repository:
   ```bash
   git clone https://github.com/yourusername/netflix-eda.git
   cd netflix-eda
