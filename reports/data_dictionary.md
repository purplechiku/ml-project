# Lab 1 - Olist E-Commerce Dataset Data Dictionary

## Overview

The Olist Brazilian E-Commerce Dataset consists of multiple related tables representing customers, orders, products, sellers, reviews, payments, and geographical information.

---
## Customers

| Column | Data Type | Description | Example |
|---------|-----------|-------------|---------|
| customer_id | String | Unique customer identifier for each order | `06b8999e...` |
| customer_unique_id | String | Unique customer identifier across multiple orders | `861eff47...` |
| customer_zip_code_prefix | Integer | Customer ZIP code prefix | `14409` |
| customer_city | String | Customer city | `franca` |
| customer_state | String | Customer state | `SP` |
## Orders

| Column | Data Type | Description | Example |
|---------|-----------|-------------|---------|
| order_id | String | Unique order identifier | `e481f51c...` |
| customer_id | String | Customer who placed the order | `9ef432eb...` |
| order_status | String | Current order status | `delivered` |
| order_purchase_timestamp | Datetime | Purchase date and time | `2017-10-02 10:56:33` |
| order_approved_at | Datetime | Payment approval time | `2017-10-02 11:07:15` |
| order_delivered_carrier_date | Datetime | Date sent to carrier | `2017-10-04 19:55:00` |
| order_delivered_customer_date | Datetime | Delivery date | `2017-10-10 21:25:13` |
| order_estimated_delivery_date | Datetime | Estimated delivery date | `2017-10-18` |
## Order Items

| Column | Data Type | Description | Example |
|---------|-----------|-------------|---------|
| order_id | String | Order identifier | `00010242...` |
| order_item_id | Integer | Item number in the order | `1` |
| product_id | String | Product identifier | `4244733e...` |
| seller_id | String | Seller identifier | `48436dad...` |
| shipping_limit_date | Datetime | Shipping deadline | `2017-09-19 09:45:35` |
| price | Float | Product price | `58.90` |
| freight_value | Float | Shipping cost | `13.29` |