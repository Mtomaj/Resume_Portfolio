# 🛒 Amazon Inventory Analysis

This project contains an exploratory data analysis (EDA) of Amazon product data, performed in Excel. The analysis focuses on exploring relationships between product ratings, discount percentages, and categories to uncover actionable insights.

## 📁 File

- **Amazon Inventory Analysis.xlsx**  
  Contains multiple Excel worksheets with data cleaning, rating group logic, and visual summaries.

---

## 🧹 Data Cleaning

Based on the original dataset from [Kaggle](https://www.kaggle.com/code/mehakiftikhar/amazon-sales-dataset-eda), the following data cleaning steps were applied:

1. **Column Selection:**  
   Removed irrelevant columns such as `img_link`, `product_link`, `about_product`, `user_id`, `user_name`, `review_id`, `review_title`, and `review_content` to simplify the analysis.

2. **Data Type Conversion:**  
   - `discounted_price`, `actual_price`, and `discount_percentage` were cleaned by removing symbols like `₹`, `,`, and `%`, then converted to numeric types.
   - `rating` and `rating_count` were also converted from text to numeric format.

4. **Category Column Splitting:**  
   - The `category` field was split into two new columns:
     - `MainCategory`
     - `SubCategory`
   - This improved flexibility when analyzing data by category.

5. **String Normalization:**  
   Standardized inconsistent category names:
   - `"Computers&Accessories"` → `"Computers Accessories"`
   - `"HomeImprovement"` → `"Home Improvement"`
   - `"MusicalInstruments"` → `"Musical Instruments"`
   - `"OfficeProducts"` → `"Office Products"`

---

## 📊 Key Features of the Analysis

- **Rating Grouping:** Products were grouped into rating buckets:  
  `1–2.9`, `3–3.9`, `4–4.5`, `4.6–5`

- **Discount Analysis:**  
  - Calculated average discount by rating group  
  - Identified trends where lower-rated products were discounted more heavily

- **Excel Techniques Used:**
  - `IF`, `AVERAGEIFS`, `COUNTIFS`, `MINIFS`
  - Structured table references (`[@ColumnName]`)
  - Power Query
  - Charting with bar graphs for rating vs. discount

---

## 🎯 Objectives

- Explore how product ratings influence discount strategies.
- Categorize performance across rating tiers.
- Prepare data for future dashboarding (e.g., Tableau or Power BI).

---

## 📈 Possible Extensions

- Import the Excel dataset into Tableau for interactive visual dashboards.
- Add price trend analysis, inventory forecasts, or deeper category-level insights.
- Connect to Amazon’s API for real-time price and stock tracking.

---

## 🧑‍💻 Skills Demonstrated

- Data cleaning and normalization
- Logical and statistical Excel functions
- Visual storytelling through charts
- Analytical reasoning and business insight generation

---

## 📬 Contact

Feel free to connect with me on [LinkedIn](https://www.linkedin.com/) or reach out via [GitHub](https://github.com/Mtomaj) if you'd like to collaborate or provide feedback!
