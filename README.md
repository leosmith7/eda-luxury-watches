# Luxury Watch Market EDA

Exploratory data analysis of 284,000+ luxury watch listings from
the secondary resale market.

## Dataset

Source: (https://www.kaggle.com/datasets/philmorekoung11/luxury-watch-listings)
Size: 284,491 listings across 14 features including brand, model,
price, movement type, case material, condition, and year of production.

## Questions Investigated

1. **Which brands dominate the resale market?**  
   Rolex leads by a wide margin, followed by Omega and Seiko.

2. **Does movement type affect price?**  
   Manual winding movements command the highest median price,
   ahead of automatic,likely reflecting their association with
   high-horology heritage pieces rather than mass-market positioning.

3. **How have prices changed over time?**  
   Median prices rise steadily from 2000-2022. The sharp swings
   in 2023-2024 are sample-size artifacts at the recent
   end of the data, not real market signals.

4. **How much does condition affect resale value?**  
   Condition is a weaker price predictor than expected, Very Good
   watches outprice New ones, suggesting brand and model drive
   price more than condition grade alone.

5. **Does case material predict price?**  
   Rose gold commands the highest prices, even above yellow gold,
   reflecting current market fashion. Steel is the lowest-priced
   but highest-volume material.

## Key Data Challenges

- 69% of movement type data missing, 58% of case material missing,
  analyses on these columns reflect a documented subset, likely
  skewed toward higher-value, more thoroughly listed watches.
- Price stored as formatted string ($43,500), required cleaning.
- Year of production required coercion to numeric, with some
  non-numeric entries dropped.

## How to Run

```bash
pip install pandas matplotlib seaborn jupyter
jupyter notebook notebooks/01_exploration.ipynb
```

## Tools

Python · Pandas · Matplotlib · Seaborn · Jupyter
