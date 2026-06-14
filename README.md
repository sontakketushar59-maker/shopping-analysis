# Shopping Dataset Analysis Project

## 1. Objective
Perform exploratory data analysis (EDA), data cleaning, and derive meaningful insights from the combined dataset using Python and Pandas.

## 2. Dataset
- Source: `combined_dataset.csv`
- Cleaned: `Cleaned_Combined_dataset.csv`
- Contains product details such as title, category, rating, ratings count, initial price, discount, and final price.

## 3. Steps Followed
1. Load dataset into Pandas DataFrame.  
2. Explore data: preview rows, check shape, column names, data types, and missing values.  
3. Clean data: remove duplicates, handle missing values, and convert numeric columns.  
4. Feature engineering:  
   - `price_difference` = initial price – final price  
   - `popularity` = rating × ratings_count  
   - `total_amount` = final price × quantity (fallback = final_price)  
5. Analysis: univariate, bivariate, and category‑level.  
6. Visualization: histograms, scatterplots, bar charts, boxplots.  
7. Insights: summarize findings and business implications.  
8. Export: save cleaned dataset as `Cleaned_Combined_dataset.csv`.  
9. Final summary: rows, columns, missing values, duplicates, new columns.

## 4. Key Insights
1. Most products are priced under ₹3000, with premium categories like watches going higher.  
2. Average rating is around 4.0, showing strong customer satisfaction.  
3. Backpacks and jeans are affordable and popular, driving high sales volume.  
4. Watches are expensive but still attract demand, making them high‑margin products.  
5. Niche categories (like yoga mats) need targeted promotions to increase visibility.  

## 5. Business Implications
1. Pricing strategy: Premium categories should be marketed for margins, while affordable ones drive volume.  
2. Recommendations: Popular products (high ratings × ratings count) are ideal for homepage features.  
3. Discount management: Large price differences highlight aggressive discounting — monitor margins.  
4. Inventory planning: Products with high `total_amount` should always be in stock.  
5. Quality control: Categories with low ratings need supplier review or delisting.  
6. Premium targeting: High‑price niche categories need focused marketing.

## 6. Project Structure
shopping-analysis/
│── data/
│   └── combined_dataset.csv
│   └── Cleaned_Combined_dataset.csv
│── notebook/
│   └── analysis.ipynb
│── README.md


## 7. How to Run
Clone the repository, install libraries, open the notebook, and run all cells. The cleaned dataset will be saved automatically.

```bash
git clone https://github.com/your-username/shopping-analysis.git
cd shopping-analysis
pip install pandas numpy matplotlib seaborn
jupyter notebook notebook/analysis.ipynb
Output file: data/Cleaned_Combined_dataset.csv
