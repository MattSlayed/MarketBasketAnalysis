# Market Basket Analysis

Retail transaction analysis using association rule mining to identify frequently purchased product combinations, enabling data-driven cross-selling strategies and store layout optimization.

## Objective

Analyze transaction data to uncover product purchase patterns using the Apriori algorithm, delivering actionable recommendations for product bundling, shelf placement, and targeted promotions.

## Key Findings

- **Top associations**: Milk & Bread, Eggs & Butter (high lift values)
- **High confidence**: Milk -> Bread — buyers of Milk are likely to also buy Bread
- **10+ high-value product associations** identified from transaction data

## Recommendations

- Offer product bundles (e.g., Milk + Bread discount)
- Place associated products in proximity on shelves
- Run targeted promotions for high-lift product pairs

## Tech Stack

- **Language**: Python (Jupyter Notebook)
- **Database**: SQLite
- **Libraries**: Pandas, mlxtend (Apriori), Matplotlib
- **Output**: CSV export of association rules

## Project Structure

```
MarketBasketAnalysis/
├── Market_Basket_Analysis.ipynb    # Main analysis notebook
├── Business_Requirements_Document.md
├── analysis_summary.txt            # Key findings summary
├── market_basket_results.csv       # Exported association rules
├── product_associations.png        # Visualization of top associations
├── Process Flow diagram.png        # Analysis workflow diagram
└── retail.db.db                    # SQLite transaction database
```

## Methodology

1. **Data extraction** — SQL queries against retail transaction database
2. **Data preparation** — Transaction encoding into basket format
3. **Association mining** — Apriori algorithm (support > 0.01, confidence > 0.5)
4. **Analysis** — Lift, confidence, and support metrics for product pairs
5. **Reporting** — Visualizations and CSV export for stakeholder review

## License

MIT
