# Design Decisions

## Microsoft Fabric
Fabric is the unified analytics platform for data engineering, lakehouse, warehouse, semantic modelling and Power BI.

## OneLake
OneLake provides centralized storage across the Fabric solution.

## Medallion Architecture
Landing, Bronze, Silver and Gold separate source delivery, raw persistence, trusted transformation and business-ready analytics.

## Bronze Preservation
Bronze uses minimal transformation so source data can be retained and reprocessed.

## Incremental Processing
`ModifiedDate` is the initial watermark candidate. A reusable control mechanism will be implemented later.

## Metadata-Driven Ingestion
The proven customer ingestion will be generalized so datasets can be onboarded through configuration rather than duplicated pipeline logic.

## Synthetic Data
Synthetic data allows public GitHub publication without exposing confidential data.

## Controlled Data-Quality Issues
Intentional bad records allow validation, quarantine, reconciliation and remediation patterns to be demonstrated.

## SCD Type 2
Historical customer/product changes will be preserved where required.

## GitHub
GitHub provides source control, documentation and portfolio visibility.
