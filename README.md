# SQL-Motiva-Autos-Project
A PostgreSQL sales and customer analytics project exploring vehicle demand, pricing tiers, revenue accumulation, and buyer segmentation for an automotive dealership.

## Table of Contents
- [Overview](#overview)
- [Problem Statement and Project Objectives](#Problem-Statement-and-Project-Objectives)
- [Selected SQL Previews](#Selected-SQL-Previews)
- [Business Applications](#Business-Applications)
- [Tech Stack](#Tech-Stack)

## Overview
MotivaAutos is a project that turns raw dealership records, spanning customer profiles, vehicle inventory, and sales transactions into structured business intelligence. Using PostgreSQL, the script moves systematically from foundational data profiling and filtering to multi-table joins, conditional segmentation, date-part trend extraction, and window-function ranking.

## Problem Statement and Project Objectives
### Problem Statement
Automotive dealerships sit on rich transactional and customer records, yet without structured querying, leadership lacks clear answers on which vehicle brands, and vehicle models drive volume, how revenue accumulates over time, which buyers generate repeat high-value orders, and where unengaged leads sit in the customer base.

### Project Objectives
- Revenue and Volume Tracking: Measure total sales revenue, total units sold, order counts, and cumulative running sales totals over time.
- Vehicle and Inventory Merchandising: Compare performance across car brands, models, price brackets (Affordable, Mid-range, Luxury), and exterior colors (car_color) to guide stocking decisions.
- Customer Segmentation: Group buyers by age demographics (Youth, Adult, Senior) and revenue-based loyalty tiers (Bronze, Silver, Gold).
- Retention and Lead Identification: Isolate high-spending VIP customers exceeding average order revenue alongside inactive accounts with zero recorded purchases.
Data Hygiene and Auditing: Detect duplicate email records, standardize missing contact or revenue values, and enforce clean data types.

## Selected SQL Previews
- Rank cars by total sales
<img width="1049" height="666" alt="1" src="https://github.com/user-attachments/assets/743b099c-95bd-49c7-a5b9-dc50217504c7" />

- Running total of sales
<img width="1049" height="681" alt="2" src="https://github.com/user-attachments/assets/a2ae9e8c-a2ed-4ae2-a4a3-56a3b6456657" />

- Customer Segmentation into Gold, Silver, Bronze
<img width="1049" height="671" alt="3" src="https://github.com/user-attachments/assets/c36ace21-9f1a-4de3-9d00-5ccfccea0e4d" />

- Total sales by car color, where total sales are above the overall average sales amount per order
<img width="1051" height="677" alt="4" src="https://github.com/user-attachments/assets/1c795f95-16a8-4ff6-a1e2-b9a9c4513656" />

- Cars sold, with their corresponding revenue and units sold
<img width="1051" height="673" alt="5" src="https://github.com/user-attachments/assets/13faab45-58a8-4a0b-8f85-242566b10364" />

## Business Applications
- Prioritize Top-Ranked Models: Use the vehicle model rankings to allocate showroom floor space and supplier orders toward high-turnover configurations.
- Target VIP Tiers & Re-Engage Zero-Order Leads: Enroll Gold and Silver tier buyers in priority service or trade-in programs, while running targeted outreach for registered customers with no order histories.
- Align Inventory & Promotions Around Seasonal Peaks: Monitor monthly revenue curves and running totals to time financing offers and inventory intake ahead of peak buying months.
- Clean CRM Contact Records: Clean flagged email addresses and prompt accounts marked 'Non-provided' to update contact details during service visits.

## Tech Stack
Database: PostgreSQL
Database Engine: PostgreSQL
- Core Querying & Filtering: SELECT, DISTINCT, WHERE, AND/OR, BETWEEN, IN, LIKE, ORDER BY, LIMIT
- Joins & Set Operations: INNER JOIN, LEFT JOIN, UNION
- Aggregations & Subqueries: SUM, COUNT, AVG, MIN, MAX, GROUP BY, HAVING, subqueries
- Window Functions & Transformations: RANK() OVER (...), windowed running totals (SUM(...) OVER (...)), CASE, COALESCE, CAST, EXTRACT, CONCAT


