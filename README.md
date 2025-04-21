# Netflix Movies and TV Shows – Data Cleaning in Excel

This project involves cleaning and preparing the **Netflix Movies and TV Shows dataset** using Microsoft Excel.

## 📁 Files

- `netflix_cleaned.xlsx` – Cleaned dataset with formatting, deduplication, and standardized columns.
- `README.md` – Summary of the cleaning tasks performed.

## 🔧 Cleaning Steps Performed

1. **Formatted Layout:**
   - Adjusted column widths and row heights
   - Enabled text wrapping for readability
   - Applied bold formatting and fill color to headers

2. **Removed Duplicates:**
   - Identified and deleted 2 duplicate rows

3. **Date Column:**
   - Standardized date format using Excel formula:
     ```excel
     =DATE(RIGHT(G2,4), MONTH(1 & LEFT(G2,FIND(" ",G2)-1)), MID(G2,FIND(" ",G2)+1, FIND(",",G2)-FIND(" ",G2)-1))
     ```

4. **Duration Column:**
   - Split into `Duration_Value` and `Duration_Unit` (e.g., `90` and `min`, `2` and `Seasons`)

5. **Missing Values:**
   - Replaced missing text entries with `NA`
   - Replaced missing numeric entries with `0`

7. **Data Types Standardized:**
   - Text columns formatted as Text (including numerical titles)
   - Date columns formatted as Date
   - Duration values set as numeric

## 🧰 Tools Used

- Microsoft Excel
- GitHub

---

## 🚀 How to Use

You can use this cleaned dataset for:

- Visualizing trends by year, rating, or duration
- Analyzing actor appearances or genre popularity
- Creating dashboards in Excel, Tableau, or Power BI

---

## 📌 Notes

- The original dataset can be found on [Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows)
- This cleaned data is ready for analysis or visualization using Excel, Tableau, or Python.