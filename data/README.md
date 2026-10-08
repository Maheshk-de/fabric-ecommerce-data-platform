# Synthetic E-Commerce Source Data

This directory contains reproducible synthetic source data for the Microsoft Fabric E-Commerce Data Platform project.

## Source simulation

- SQL Server: customers.csv, products.csv, stores.csv
- CSV/SFTP: sales.csv, inventory.csv, returns.csv
- REST/JSON: promotions.json

## Intentional data-quality issues

The source data intentionally contains a small number of:
- duplicate records
- null business keys/attributes
- invalid foreign keys
- invalid email formats
- negative quantities/stock/refunds
- products where UnitPrice < UnitCost

These issues are intentional and will be handled in the Silver/data-quality layer.
