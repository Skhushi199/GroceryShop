# 🛒 Market Basket Analysis with Apriori

This project applies **Association Rule Mining** using the **Apriori algorithm** (via the `apyori` library) to uncover relationships between products in a supermarket dataset. The goal is to identify frequent itemsets and generate rules that highlight which products are often purchased together.

---

## 📂 Dataset
- **File:** `Market_Basket_Optimisation.csv`
- **Rows:** 7,501 transactions
- **Columns:** Up to 20 items per transaction
- **Description:** Each row represents a customer’s basket of items purchased.

---

## ⚙️ Methodology
1. **Data Preprocessing**
   - Loaded the dataset using `pandas`.
   - Converted each transaction into a list of items.

2. **Apriori Algorithm**
   - Implemented using the `apyori` library.
   - Parameters used:
     - `min_support = 0.003`  
     - `min_confidence = 0.2`  
     - `min_lift = 3`  
     - `min_length = 2`  
     - `max_length = 2`

3. **Rule Generation**
   - Extracted association rules showing product pairs with strong support, confidence, and lift.
   - Converted results into a `pandas` DataFrame for easy analysis.

---

## 📦 Dependencies
Make sure you have the following installed:
```bash
pip install pandas numpy matplotlib apyori
