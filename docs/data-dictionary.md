# Source Data Dictionary

| Dataset | Source Simulation | Key | Incremental Column |
|---|---|---|---|
| customers | SQL Server | CustomerID | ModifiedDate |
| products | SQL Server | ProductID | ModifiedDate |
| stores | SQL Server | StoreID | ModifiedDate |
| sales | CSV/SFTP | OrderID | ModifiedDate |
| inventory | CSV/SFTP | InventoryID | ModifiedDate |
| returns | CSV/SFTP | ReturnID | ModifiedDate |
| promotions | REST/JSON | PromotionID | ModifiedDate |

## Target Analytical Model

### Dimensions
- dim_customer
- dim_product
- dim_store
- dim_date
- dim_promotion

### Facts
- fact_sales
- fact_inventory
- fact_returns

## Source Domains
- Customers: customer identity, contact and location.
- Products: category, brand, cost and selling price.
- Stores: location and store type.
- Sales: transactional order-line data.
- Inventory: daily stock movement.
- Returns: returned-order transactions.
- Promotions: product-linked promotional campaigns.
