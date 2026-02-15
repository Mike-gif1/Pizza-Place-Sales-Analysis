# Data Analysis Guide

## Overview
This guide explains the analysis methodology and how to interpret the results.

## Data Processing Steps

### 1. Data Loading
- Extract CSV files from the zip archive
- Validate file integrity and completeness

### 2. Data Merging
```
order_details (pizza_id) → pizzas → pizza_types (pizza_type_id)
order_details (order_id) → orders
```

### 3. Feature Engineering
- **Date/Time Features:** Extract hour, day of week, month, and quarter
- **Revenue Calculation:** quantity × price

## Key Metrics Explained

### Total Revenue
Sum of all (quantity × price) across all orders

### Average Order Value
Total revenue divided by the number of unique orders

### Peak Hours
Hours with highest revenue and order volume

### Category Performance
Revenue and quantity distribution across pizza categories

## Interpretation Guide

### Peak Hours Analysis
- **Use for:** Staffing schedules, inventory planning
- **Action Items:** Increase resources during peak hours

### Weekly Patterns
- **Use for:** Marketing campaigns, promotional planning
- **Action Items:** Target promotions to slower days

### Seasonal Trends
- **Use for:** Annual planning, budget forecasting
- **Action Items:** Prepare for seasonal fluctuations

### Product Analysis
- **Bestsellers:** Promote, feature in bundles
- **Low Performers:** Discount, improve, or discontinue

## Best Practices

1. **Update Regularly:** Refresh analysis monthly for trend monitoring
2. **Combine Insights:** Use multiple metrics for holistic decisions
3. **Context Matters:** Consider external factors (holidays, events, weather)
4. **Test Changes:** Implement recommendations gradually with measurement

## Glossary

- **Revenue:** Total monetary value of sales
- **Quantity:** Total number of items sold
- **Order:** Single customer transaction (may contain multiple items)
- **Category:** Pizza type classification (e.g., Vegetarian, Meat, etc.)