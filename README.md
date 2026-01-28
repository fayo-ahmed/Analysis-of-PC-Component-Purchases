# Analysis-of-PC-Component-Purchases

## Overview
This project analyzes PC component purchasing behavior using association rule mining
to identify co-purchase patterns that can support inventory planning, product bundling,
and targeted promotions.

## Data
- ~10,000 transactional records of PC component purchases
- Each transaction represents a complete PC build

## Methodology
- Data cleaning and transaction encoding using pandas and TransactionEncoder
- Frequent itemset mining with Apriori (min_support = 0.02)
- Association rule generation with confidence ≥ 0.2
- Rule evaluation using lift to identify meaningful associations
- Visualization of support vs confidence colored by lift

## Key Results
- Identified high-support rules representing common purchasing behavior (e.g., CPU → Motherboard)
- Discovered lower-support but higher-lift rules indicating stronger co-purchase dependencies
- Observed a tradeoff between rule frequency and rule strength across itemsets

## Business Implications
- High-support rules can guide inventory prioritization for core components
- High-lift rules provide opportunities for targeted promotions and bundling strategies
- Results can support demand planning and recommendation-style systems

## Technologies Used
- Python, pandas, NumPy
- mlxtend (Apriori, association rules)
- Matplotlib
