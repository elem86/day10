# Day 10

🎯 Day 10 – One Project a Day Until I Get Hired

🧩 SQL Project: CTEs for Cleaner Queries

Today’s focus was on improving SQL query structure and readability by using Common Table Expressions (CTEs). These are great for breaking down complex logic into manageable steps — especially useful when dealing with grouped and aggregated data.


✅ What I built:

 - Created a mock revenue table with 200+ rows of product, category, and sales data

 - Used a CTE to calculate total sales by product and category

 - Queried the CTE to display and sort results by total revenue

💡 Why it matters:
CTEs let you write more readable and maintainable SQL — especially when building layered queries. They're also useful for performance when reused multiple times in the same query.

🔍 Sample CTE used:
<pre> ```sql
WITH product_sales AS (
  SELECT
    product_name,
    category,
    SUM(sales) AS total_sales
  FROM revenue
  GROUP BY product_name, category
)
SELECT *
FROM product_sales
ORDER BY total_sales DESC;
``` </pre>
⏱ This was a quick 1-hour build — a perfect warm-up before moving into more advanced logic like ranking and de-duplication tomorrow!

📂 Files on GitHub: 🔗 https://github.com/elem86/day10

#SQL #CTE #DataAnalytics #JobSearch #OpenToWork #Day10 #LearnSQL #DataAnalysis #OpenToWork #OneProjectADay #LinkedInLearning
