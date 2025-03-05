# OpenFoodFacts Morocco Analysis

## 1. Data Extraction & Filtering
- Loaded the **OpenFoodFacts dataset** from a Parquet file.
- Filtered the data to include only products related to **Morocco**, based on multiple fields (`countries_tags`, `main_countries_tags`, `origins_tags`, `manufacturing_places`).
- **Result:** 14,652 products matching Moroccan-related tags.
- Saved the filtered dataset in a **Parquet file** for further analysis.

## 2. Category Analysis
- Identified **top 10 product categories** based on their occurrence in the dataset.
- The most frequent category had **9,457 NULL values**, followed by categories like **Snacks, Dairy Products, and Confectionery**.
- Saved the category breakdown in a Parquet file.

## 3. Brand & Product Popularity
- Ranked brands by **product count** in Morocco.
- Extracted **top 10 brands** with the highest number of products.
- Attempted to analyze **product count per brand**, but execution was canceled.

## 4. Nutritional Analysis
- Grouped products by **Nutriscore Grade** (A to E).
- Found **345 products with Nutriscore 'A' (healthiest) and 894 with Nutriscore 'E' (least healthy)**.
- Extracted and saved details (name, brand, OpenFoodFacts URL) of **Nutriscore 'A' products**.

## 5. Additives & Allergens
- Analyzed **additives** usage across products.
- Attempted to identify products with **zero additives**, but execution was canceled.

## 6. Geographical & Time-Based Insights
- Explored **cities** where products are available.
- Analyzed **last update timestamps** to see how frequently Moroccan product data is updated.
- Some geographical insights queries were canceled before execution.

## Suggested KPIs & New Descriptive Analyses
### 1. Product Completeness Score
- Evaluate the **completeness** of product data (how many key fields are missing per product).
- KPI: **% of products with more than X missing fields**.

### 2. Most Common Ingredients
- Extract and rank **most frequently used ingredients** in Moroccan products.
- KPI: **Top 10 ingredients by frequency**.

### 3. Nutriscore Trend Over Time
- Analyze how Nutriscore distribution has changed over the years.
- KPI: **Average Nutriscore per year**.

### 4. Organic vs. Non-Organic Products
- Compare product counts with and without **organic** labels.
- KPI: **% of organic products in Moroccan dataset**.

### 5. Product Recency Index
- Measure how up-to-date product data is.
- KPI: **% of products updated in the last X months**.

### 6. Popularity Score Analysis
- Examine **unique scans and purchase places** to determine the most popular products.
- KPI: **Top 10 most scanned products in Morocco**.

These analyses will help refine insights and improve the dataset's usability. 🚀
