## Feature-Engineering-to-Predicted-Freight-Delay-Risk
Engineered logistic and financial features to build a Random Forest model that predicts freight delivery delays using supply chain data. The model enabled risk-based insurance pricing, calculating premiums that balance expected claims, fixed costs, and profit margins.

# Feature Engineering Summary

| Engineered Feature               | Description                                                                 |
|----------------------------------|-----------------------------------------------------------------------------|
| `Average Order Value`           | Sales per order, calculated from order item totals                         |
| `Discount_Impact`               | Estimated financial impact of discounts on order profitability             |
| `Order_Value_per_Quantity`      | Normalized order value by quantity to detect order complexity              |
| `Order_Value_to_Quantity_Ratio` | Captures efficiency of value shipped per unit ordered                      |
| `Avg_Sales_Segment`             | Average sales segmented by customer or product group to reflect priority   |

