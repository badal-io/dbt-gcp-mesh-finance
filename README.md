# dbt Mesh Finance

## Models Overview

This dbt project contains data marts for financial and order analytics within the Jaffle Shop mesh architecture. All models are owned by the finance team and leverage staging data from the platform group.

### Models

- **order_items** - Detailed order item data with product pricing, supply costs, and item categorization (food/drink). One row per order item.
- **orders** - Order summary data mart with cost analysis, order totals, and food/drink breakdowns. One row per order.
- **products** - Product reference data sourced from the platform staging layer.
- **supplies** - Supply data including costs, sourced from the platform staging layer.

The models follow a layered architecture where raw platform data is transformed into business-ready finance marts with proper contracts and data quality tests.