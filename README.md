# MarketUZ — SSAS Tabular Data Model

## Project Overview

This project implements an SQL Server Analysis Services (SSAS) Tabular model for analyzing wholesale sales data from MarketUZ for 2022–2025.

The model is designed to support sales reporting, profitability analysis, customer insights, and time-based analysis using DAX measures.

## Data Model

The model contains six tables:

- `FactOrders` — sales transaction data
- `DimDate` — calendar and date attributes
- `DimProduct` — product information
- `DimCustomer` — customer information
- `DimWarehouse` — warehouse information
- `DimEmployee` — employee information

The model uses a star-schema-style structure, with `FactOrders` connected to the relevant dimension tables through relationships.

## Key Metrics

The model includes DAX measures for:

- Total Revenue
- Total Cost
- Gross Profit
- Margin %
- Total Quantity
- Order Count
- Average Order Value
- Total Discount
- Discount %
- Return Lines
- Revenue % of Total
- Revenue % of Category
- Revenue Previous Year
- Year-over-Year Growth %
- Revenue Year-to-Date
- Top Customer Name

## Tools and Technologies

- Microsoft SQL Server
- SQL Server Analysis Services (SSAS) Tabular
- Visual Studio
- DAX
- Microsoft Excel PivotTables
- Git and GitHub

## Validation

The model was processed and deployed successfully. Its results were validated against SQL queries and reviewed using an Excel PivotTable connected to the Tabular model.

Validated metrics include total revenue, distinct order count, and 2024 revenue.

## Repository Contents

- `MarketUZ_Tabular.sln` — Visual Studio solution
- `MarketUZ_Tabular.smproj` — SSAS Tabular project
- `Model.bim` — Tabular model definition

## Purpose

This project demonstrates practical skills in dimensional modeling, DAX measure development, SSAS Tabular deployment, and analytical reporting.
